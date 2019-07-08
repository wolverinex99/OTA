# LotusOS
## Official devices application

[Official Support Application](https://docs.google.com/forms/d/e/1FAIpQLSfSicVS1xXCmalXCpHQF5BqD2MfW4nko0gpNGoeARaIT48njg/viewform) 
|
[Devices Repository](https://github.com/LotusOS-Devices)

Before you submit a pull request to add your device to our list of official devices, you should know a few simple things:

### 1. To become a maintainer of LotusOS:

1.2 - You must have a way to check your builds. Either owning the device, or sending builds to a reliable/trusted person to test for you. Completely blind and/or untested builds are not permitted.

1.3 - Applicants that physically own the device, will have the preference on receiving maintainship.

1.4 - You must have knowledge of git.

1.5 - You must compile an unofficial build and make the device stable for daily usage before applying.

1.6 - You should have your device sources publicly available for us take a look at.

1.7 - You mustn't be a placeholder of another maintainer that was removed. Pull request's considered of that nature won't be accepted.

### 2. Maintainers code of conduct:

2.1 - Maintainers MUST import their trees to https://github.com/LotusOS-Devices

2.2 - Maintainers MUST test every update before uploading/Pushing OTA.

2.3 - Maintainers MUST keep the authorship of Git commits, even if it's your device tree, kernel or ROM source. Lots of git commit --amend and force-pushes are acceptable.

2.4 - Relationships fights can be done in PM on Telegram or XDA. 

2.5 - Maintainers also need to add/execute 'export LOTUS_BUILD_TYPE=OFFICIAL' in/to their build environment in order to compile as official with OTA application.

### 3. JSON params

##### devices.json
| Param | Description | Required |
|--|--|--|
| name | Device name | Yes |
| brand | Device manufacturer | Yes |
| codename | Device codename, eg: falcon | Yes |
| version_code | Version code, lowercase, eg: oreo | Yes |
| version_name | Version name, will be shown on download portal, eg: Oreo | Yes |
| maintainer_name | Your name | Yes |
| maintainer_url | Your personal URL, eg: https://github.com/hungphan2001 or https://forum.xda-developers.com/member.php?u=7504475 | No  |4936496
| xda_thread | XDA thread URL, eg:  | No |

##### builds/your_device_codename.json
| Param | Description | Required |
|--|--|--|
| filename | Build file (.zip) name | Yes |
| filesize | Build file (.zip) size (in bytes) | Yes |
| filehash | Build file (.zip) md5 hash | Yes |
| datetime | Build file (.zip) time | Yes |
| id | Build file (.zip)  hash | Yes |
| forum_url | XDA Thread | Yes |
| telegram_username | Your telegram usrname | Yes |

