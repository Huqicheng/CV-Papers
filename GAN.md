# GAN

## 1. GAN

#### 1.1 Structure

[GAN](http://ss.csdn.net/p?https://mmbiz.qpic.cn/mmbiz_png/iaTa8ut6HiawCUoIVNsXpWVcLibMiaesQkjxuxMTNqrJJy7A9mNicyyGwqWmKJWUseJgBhlNOKBIOc9B3Gr64umFrJA/0?wx_fmt=png)

#### 1.2 Loss

generator: mean[log(D(x)) + log(1-D(G(z)))]

discriminator: mean[log(1-D(G(z))]

where z is results of generator and x is the real data.

## 2.DCGAN

## 3. WGAN

#### 3.1 Wasserstein Distance

For improving and stablizing the training process of GAN.

```python
self.D_loss = - tf.reduce_mean(self.D_real) + tf.reduce_mean(self.D_fake)
self.G_loss = - tf.reduce_mean(self.D_fake)
```
