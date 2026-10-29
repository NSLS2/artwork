# NSLS-II Beamline Artwork

---

Permission is granted to use the Brookhaven images in this repository.
Permission is applicable only for the the images in the document. Without
limitation, the images shall not be utilized to endorse, or imply
endorsement of any product or service.  Images may not be digitally
manipulated in any way except to adjust size, crop or color attributes
to optimize it for print production.  The credit line "Courtesy
of Brookhaven National Laboratory" shall be included with the images
or as a separate credit adjacent to the image.
Usage of the image constitutes your agreement with these terms.

---

## Slack icons

The `turtle/icons/` directory holds icons for NSLS-II Slack apps and
workflows. Each one is the NSLS-II turtle with a single bold mark in the
centre of its ring, so the apps look like a family and are told apart by
their mark. The icons are teal (`#105C78`, the BNL primary colour); alerts
use red (`#CC0000`).

Every icon comes in three sizes: `NAME-1024.png` (upload this to Slack),
`NAME-512.png` (the smallest size Slack accepts) and `NAME-128.png`
(custom emoji).

| Icon | Mark | Used for |
| --- | --- | --- |
| `slack-admin-icon` | Gear | NSLS2 Slack Admin app |
| `docassist-icon` | Open book | DocAssist app |
| `nsls2workflows-icon` | Nodes and arrow | `nsls2workflows` app |
| `opmon-icon` | Megaphone | NSLS-II Operations Monitor app |
| `docs-messages-icon` | Speech bubble | N2SN Docs Messages app |
| `aifapim-workflow-icon` | Key and sparkles | Request an AIFAPIM key workflow |
| `github-copilot-workflow-icon` | Code brackets and sparkles | Request GitHub Copilot workflow |
| `notifications-workflow-icon` | Megaphone with waves | Notifications workflow |
| `travel-workflow-icon` | Airplane | Travel workflow |
| `dssi-outage-notification-icon` | Warning triangle (red) | DSSI outage notification workflow |

New icons can be made with the `nsls2-artwork` skill.

## Installation

The artwork can bin installed using the Makefile provided.

```shell
$ make
$ make install
```

## Building Debian Package

The debian package can be built from this git repository by executing:

```shell
$ gbp buildpackage --git-debian-branch=main -uc -us  --git-export-dir=build
```

which will build the package in the directory `./build`
