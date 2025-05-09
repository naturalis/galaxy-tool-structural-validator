# galaxy-tool-structural-validator
Galaxy tool for structural validation of DNA barcode data

How to submit a tool to the Galaxy ToolShed:

1. Create an account on the [ToolShed](https://toolshed.g2.bx.psu.edu/)
2. Create a $HOME/.planemo.yml file with the following content:

```yaml
shed_username: $USER # your ToolShed username
sheds:
  toolshed:
    key: $KEY        # your ToolShed API key, under 'User > API Keys'
    email: $EMAIL    # your ToolShed email
    password: $PASS  # your ToolShed password
```

3. Install Planemo:

```bash
pip install planemo
```

4. Validate your tool XML:

```bash
planemo lint structural_validator.xml
```

5. Test your tool:

```bash
planemo test structural_validator.xml
```

6. Publish your tool:

```bash
planemo shed_create --shed_target toolshed
```

7. Update your tool:

```bash
planemo shed_update --shed_target toolshed
```