<div align="center">
    <h1>Watt TF Build Action</h1>
    <p>Simply run Watt TF from your GitHub Actions workflow.</p>
    <p>
        <a href="https://github.com/devsebastianops/watt-tf-build-action/actions"><img src="https://img.shields.io/github/actions/workflow/status/devsebastianops/watt-tf-build-action/on-pull-test-action.yaml?branch=main&style=flat-square" alt="CI Status"></a>
        <a href="https://github.com/devsebastianops/watt-tf-build-action/releases"><img src="https://img.shields.io/github/v/release/devsebastianops/watt-tf-build-action?style=flat-square" alt="Latest Release"></a>
        <a href="https://github.com/devsebastianops/watt-tf-build-action/blob/main/LICENSE"><img src="https://img.shields.io/github/license/devsebastianops/watt-tf-build-action?style=flat-square" alt="License"></a>
    </p>
    <h3>
    <a href="https://github.com/devsebastianops/watt-tf">Watt TF GitHub</a>
    <span> | </span>
    <a href="https://watt-tf.dev">Documentation</a>
  </h3>
</div>

---

## Inputs


| Name | Description | Required | Default |
|------|-------------|----------|---------|
| `version` | The version of Watt TF to use (e.g. latest or v1.0.0) | `false` | `'latest'` |
| `input` | The input file as JSON or YAML | `true` | |
| `blueprint` | The blueprint with the transformation rules | `true` | |
| `output` | Where should Watt TF put the .tf.json result | `true` | |
| `schema` | Optional JSON schema file for input validation | `false` | |
| `strict` | Run Watt TF build in strict mode | `false` | `'false'` |
| `stripNulls` | Run Watt TF build with strip-nulls flag | `false` | `'false'` |
| `logFormat` | Optional log format (json or text) | `false` | `'text'` |

---

## Example Usage

```yaml
  uses: devsebastianops/watt-tf-build-action@v1
  with:
    version: 'latest'
    input: '/path/to/input.json'
    blueprint: '/path/to/blueprint.yaml'
    output: '/path/to/output.tf.json'
```


---

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.


---

<p align="center">
  Made with ❤️ by <a href="https://github.com/devsebastianops">devsebastianops</a>. Happy Terraforming! 🚀
</p>
