# Neural Networks

## Functions

These functions wrap the equivalent in [jax.nn][]:

::: haliax.nn.relu
::: haliax.nn.relu6
::: haliax.nn.sigmoid
::: haliax.nn.softplus
::: haliax.nn.soft_sign
::: haliax.nn.silu
::: haliax.nn.swish
::: haliax.nn.log_sigmoid
::: haliax.nn.leaky_relu
::: haliax.nn.hard_sigmoid
::: haliax.nn.hard_silu
::: haliax.nn.hard_swish
::: haliax.nn.hard_tanh
::: haliax.nn.elu
::: haliax.nn.celu
::: haliax.nn.selu
::: haliax.nn.gelu
::: haliax.nn.quick_gelu
::: haliax.nn.glu
::: haliax.nn.logsumexp
::: haliax.nn.log_softmax
::: haliax.nn.softmax
::: haliax.nn.standardize
::: haliax.nn.one_hot

### Loss Functions

::: haliax.nn.cross_entropy_loss
::: haliax.nn.cross_entropy_loss_and_log_normalizers


## Modules

Haliax provides a small number of neural network modules that are compatible with Equinox, though
they naturally all use [haliax.NamedArray][]. (We welcome PRs for more modules! Nothing too exotic though.)
The most interesting of these modules is [haliax.nn.Stacked][], which allows you to create homogenous "stacks"
of the same module (e.g. transformer blocks), which is a common pattern in deep learning.

::: haliax.nn.Embedding
::: haliax.nn.Linear
::: haliax.nn.Dropout
::: haliax.nn.LayerNorm
::: haliax.nn.Stacked

## Attention

We don't provide an explicit attention module, but we do provide an attention function and several related functions:

:::haliax.nn.attention.dot_product_attention
:::haliax.nn.attention.dot_product_attention_weights

### Masks
::: haliax.nn.attention.causal_mask
::: haliax.nn.attention.prefix_lm_mask
::: haliax.nn.attention.combine_masks_and
::: haliax.nn.attention.combine_masks_or
::: haliax.nn.attention.forgetful_causal_mask

### Biases

::: haliax.nn.attention.mask_to_bias
::: haliax.nn.attention.alibi_attention_bias


## API Reference

::: haliax.nn
