# Rubrik Provider for Terraform

- Website: https://www.terraform.io
- [![Gitter chat](https://badges.gitter.im/hashicorp-terraform/Lobby.png)](https://gitter.im/hashicorp-terraform/Lobby)
- Mailing list: [Google Groups](http://groups.google.com/group/terraform-tool)

<img src="https://cdn.rawgit.com/hashicorp/terraform-website/master/content/source/assets/images/logo-hashicorp.svg" width="600px">


# :hammer: Installation

Requirements: Terraform has been successfully [installed](https://learn.hashicorp.com/terraform/getting-started/install.html).


1. Download the latest compiled binary from [GitHub releases](https://github.com/rubrikinc/rubrik-provider-for-terraform/releases).
   ```
   macOS: terraform-provider-rubrik-darwin-amd64
   Linux: terraform-provider-rubrik-linux-amd64
   Windows: terraform-provider-rubrik-windows-amd64.exe
   ```

2. Move the Rubrik provider into the correct Terraform plugin directory
   
   ```
   macOS: ~/.terraform.d/plugins/darwin_amd64
   Linux: ~/.terraform.d/plugins/linux_amd64
   Windows: %APPDATA%\terraform.d\plugins\windows_amd64
   ```
   
   _You may need to manually create the `plugin` directory._

3. Rename the the Rubrik provider to `terraform-provider-rubrik`

4. Run `terraform init` in the directory that contains your Terraform configuration file (`main.tf`)

# :blue_book: Documentation

Here are some resources to get you started! If you find any challenges from this project are not properly documented or are unclear, please [raise an issue](https://github.com/rubrikinc/rubrik-provider-for-terraform/issues/new/choose) and let us know! This is a fun, safe environment - don't worry if you're a GitHub newbie! :heart:

* [Quick Start Guide](https://github.com/rubrikinc/rubrik-provider-for-terraform/blob/master/docs/quick-start.md)
* [Rubrik Provider for Terraform Documentation](https://rubrik.gitbook.io/terraform-provider-for-rubrik/)
* [Rubrik API Documentation](https://github.com/rubrikinc/api-documentation)
* [VIDEO: Getting Started with the Rubrik Provider for Terraform](https://www.youtube.com/watch?v=kV1xiP1tHY0)
* [BLOG: Using Terraform with Rubrik Just Got Easier!](https://www.rubrik.com/blog/rubrik-provider-terraform/)

## :mag: Example 

```hcl
provider "rubrik" {}

resource "rubrik_configure_timezone" "LA-Timezone" {
  timezone = "America/Los_Angeles"
}
```

# :muscle: How You Can Help

We glady welcome contributions from the community. From updating the documentation to adding more functions for Terraform, all ideas are welcome. Thank you in advance for all of your issues, pull requests, and comments! :star:

* [Contributing Guide](CONTRIBUTING.md)
* [Code of Conduct](CODE_OF_CONDUCT.md)

# :pushpin: License

* [MIT License](LICENSE)

# :point_right: About Rubrik Build

We encourage all contributors to become members. We aim to grow an active, healthy community of contributors, reviewers, and code owners. Learn more in our [Welcome to the Rubrik Build Community](https://github.com/rubrikinc/welcome-to-rubrik-build) page.
