# What's this?

This custom node forcibly disables the `weights_only` option in `torch.load`.

Recently, for security reasons, `torch` has enforced the `weights_only` option when loading models to prevent arbitrary code execution embedded in model files.

Unfortunately, there are various models that require code execution, and custom nodes need to handle this properly.

However, since many custom nodes are currently unable to handle this correctly, this feature is provided as a temporary measure to disable the restriction.

# Install
Go to the `ComfyUI/custom_nodes` directory in the terminal,
and execute the following command:
```
git clone https://github.com/ltdrdata/comfyui-unsafe-torch
```

# NOTE
This extension does not include any nodes; simply install this and restart ComfyUI to see the effects.
