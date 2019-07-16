# AE

- 細かい記法は省略

## 重み共有

```

class Autoencoder(Chain):
    def __init__(self, inputs, hidden, denoising = False):
        initializer = chainer.initializers.HeNormal()
        super(Autoencoder, self).__init__(
            encoder = L.Linear(inputs, hidden, initialW = initializer),
        )
        self.add_param('b_dec', (inputs,), np.float32, chainer.initializers.Constant(0))

    def __call__(self, x):
        h = self.encoder(x)
        y = self.decoder(h)

        loss = F.mean_squared_error(y, x)
        return y, loss

    def encoder(self, x):
        return F.sigmoid(self.encoder(x))

    def decoder(self, h):
        return F.sigmoid(F.linear(h, F.transpose(self.encoder.W), self.b_dec))
```
