Chocolatey Packages (FerventCoder)
==================================

This repository contains packages that are maintained by Wilson Mar, both automatic and manually.

(based on https://github.com/ferventcoder/chocolatey-packages/blob/master/ReadMe.md)

To create a Chocolatey package using NuGet:

1. Install git client on your machine
2. navigate to the git projects folder
3. git clone https://github.com/chocolatey/chocolateytemplates.git
4. Replace your name and repository as per https://github.com/wilsonmar/chocolateytemplates

  ```
    cinst warmup
    warmup addTextReplacement __CHOCO_PKG_MAINTAINER_NAME__ "Your Name"
    warmup addTextReplacement __CHOCO_PKG_MAINTAINER_REPO__ "Your Repository (contains your packages)"
    git clone https://github.com/chocolatey/chocolateytemplates.git
    cd chocolateytemplates\_templates
    warmup addTemplateFolder chocolatey "$pwd\chocolatey"
    warmup addTemplateFolder chocolatey3 "$pwd\chocolatey3"
    warmup addTemplateFolder chocolateyauto "$pwd\chocolateyauto"
    warmup addTemplateFolder chocolateyauto3 "$pwd\chocolateyauto3"
    ```

