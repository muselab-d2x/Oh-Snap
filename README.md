# Oh Snap!
![MuseLab D2X Logo](https://github.com/user-attachments/assets/0146c305-ffd6-4651-a25f-910f6fd68e1c)

This project is a demonstration of the potential to deeply integrate Salesforce DevOps into GitHub, eliminating the need for any external platform, taking full advantage of GitHub scalability and security, and opening the door to the [Composable Delivery Model](https://muselab.com/bench-notes/introducing-the-composable-delivery-model).

This repository was created using Muselab's [D2X Launchpad](https://launchpad.muselab.com) and has been heavily edited since. 

The entire workflow being developed will soon be available for launch via D2X Launchpad. Modular, composable Salesforce development aligned with D2X's values of **Easy, Efficient, and Extensible**!

More background on the technical challenges we're tackling here:
* [Develop, Test, and Fix Faster with Scratch Org Snapshots](https://muselab.com/bench-notes/develop-test-and-fix-faster-with-scratch-org-snapshots)
* [Securing Salesforce DevOps: Least Privilege Access Control](https://muselab.com/bench-notes/securing-salesforce-devops-least-privilege-access-control)
* [5 Critical Security Questions to Ask Your SI Partner](https://muselab.com/bench-notes/5-critical-security-questions-to-ask-your-si-partner)
* [Securing Salesforce DevOps: Multi-Job Workflows in GitHub Actions](https://muselab.com/bench-notes/securing-salesforce-devops-multi-job-workflows-in-github-actions)

# Project Setup
This project is preconfigured with D2X for a comprehensive Development-to-Delivery Experience including CI/CD using GitHub Actions and development environments using GitHub Codespaces.

D2X requires some minimal configuration of your GitHub organization or repository to complete the setup and enable builds:
* [Configure Secrets](https://d2x.readthedocs.io/en/latest/tutorial/#secrets)
* [Develop Your First Change](https://d2x.readthedocs.io/en/latest/tutorial/#develop)
* [Merge Your First Change](https://d2x.readthedocs.io/en/latest/tutorial/#merge)
* [Release Your First Change](https://d2x.readthedocs.io/en/latest/tutorial/#release)

You can check the status of your setup by monitoring the status of the following GitHub Actions workflows:
* [![2GP Feature Test](https://github.com/muselab-d2x/Oh-Snap/actions/workflows/feature.yml/badge.svg)](https://github.com/muselab-d2x/Oh-Snap/actions/workflows/feature.yml)
* [![Beta Test](https://github.com/muselab-d2x/Oh-Snap/actions/workflows/beta.yml/badge.svg)](https://github.com/muselab-d2x/Oh-Snap/actions/workflows/beta.yml)
* [![Production Release](https://github.com/muselab-d2x/Oh-Snap/actions/workflows/release.yml/badge.svg)](https://github.com/muselab-d2x/Oh-Snap/actions/workflows/release.yml)

# Important Note
The `request-login-url.yml` workflow requires the `SFDX_AUTH_URL` environment variable to be set. Ensure that this variable is correctly configured in your GitHub repository secrets to avoid any issues during the login URL generation process. Additionally, the Slack API token used in the workflow must have the `chat:write:bot` scope to successfully send messages.
