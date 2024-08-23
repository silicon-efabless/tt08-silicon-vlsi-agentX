![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg) ![](../../workflows/test/badge.svg) ![](../../workflows/fpga/badge.svg)

# Tiny Tapeout Verilog Project : RTL2GDS using Agentic Flow

## Project Description
- [Read the documentation for project](docs/info.md)

## Acknowledgement

## Helpful Info

- To **locally harden** (RTL2GDS) the project, follow the [TinyTapeout Guide](https://tinytapeout.com/guides/local-hardening/). This document seems to be in a flux while TT is moving to OpenLane2. Few tweaks needed (as of 08/15/24):
  - The recommendation for Python version is 3.11 but my 3.10.12 seems to run fine. Was confirmed by the developers on the discord channel. May make a difference during reporting is what the developers think.
  - Install `python3-tk` to solve _module tkinter not found_ error: `sudo apt install python3-tk`
  - Docker needs to be installed. When installing Docker, you should choose the "_WSL2 integration_" (default) option instead of Hyper-V.
  - **Note** The above option will integrate with the default distro. If you have multiple distros (eg. Ubuntu-20.04 and 22.04) and you are running the hardening on a non-default distro, you need to set that in the Docker settings: `Settings -> Resources -> WSL Integration` and _enable_ the integration for the used distro.


# What is Tiny Tapeout?

Tiny Tapeout is an educational project that aims to make it easier and cheaper than ever to get your digital and analog designs manufactured on a real chip.

To learn more and get started, visit https://tinytapeout.com.

## Setting up your Verilog project

1. Add your Verilog files to the `src` folder.
2. Edit the [info.yaml](info.yaml) and update information about your project, paying special attention to the `source_files` and `top_module` properties. If you are upgrading an existing Tiny Tapeout project, check out our [online info.yaml migration tool](https://tinytapeout.github.io/tt-yaml-upgrade-tool/).
3. Edit [docs/info.md](docs/info.md) and add a description of your project.
4. Adapt the testbench to your design. See [test/README.md](test/README.md) for more information.

The GitHub action will automatically build the ASIC files using [OpenLane](https://www.zerotoasiccourse.com/terminology/openlane/).

## Enable GitHub actions to build the results page

- [Enabling GitHub Pages](https://tinytapeout.com/faq/#my-github-action-is-failing-on-the-pages-part)

## Resources

- [FAQ](https://tinytapeout.com/faq/)
- [Digital design lessons](https://tinytapeout.com/digital_design/)
- [Learn how semiconductors work](https://tinytapeout.com/siliwiz/)
- [Join the community](https://tinytapeout.com/discord)
- [Build your design locally](https://www.tinytapeout.com/guides/local-hardening/)

## What next?

- [Submit your design to the next shuttle](https://app.tinytapeout.com/).
- Edit [this README](README.md) and explain your design, how it works, and how to test it.
- Share your project on your social network of choice:
  - LinkedIn [#tinytapeout](https://www.linkedin.com/search/results/content/?keywords=%23tinytapeout) [@TinyTapeout](https://www.linkedin.com/company/100708654/)
  - Mastodon [#tinytapeout](https://chaos.social/tags/tinytapeout) [@matthewvenn](https://chaos.social/@matthewvenn)
  - X (formerly Twitter) [#tinytapeout](https://twitter.com/hashtag/tinytapeout) [@tinytapeout](https://twitter.com/tinytapeout)
