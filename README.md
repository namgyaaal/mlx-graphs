This is a heavy reduction of `mlx-graphs` that allows it 
- to work with `uv` ([torch_cluster currently doesn't](https://github.com/rusty1s/pytorch_cluster/issues/251))
- works with later `mlx` versions so that it can be used alongside `mlx-embeddings`

It removes tests, docs and benchmarks and removes `mlx_cluster` as a dependency and node2vec related files due to the circular dependency with it and `mlx-graphs` and it requiring an mlx version that doesn't exist on pypi. 

Use at your own discretion. I do not promise that this works except for what I'm using it for. 