# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Pr_Comments/PR-1`
- **Build Number:** #1
- **Build Status:** 🔴 **FAILURE**
- **Duration:** 4 min 7 sec and counting
- **Timestamp:** 2025-11-13 21:52:51 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 565d84f4e86c6c446b37591d4f820e1425f28e0a
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/integrations-garage/blackduck-logs-publisher
 > git init /Users/madhusud/.jenkins/workspace/Github_Coverity_Pr_Comments_PR-1@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb # timeout=10
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
 > git config --add remote.origin.fetch +refs/heads/*:refs/remotes/origin/* # timeout=10
Avoid second fetch
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
First time build. Skipping changelog.
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/coverity-cnc-jenkins-samples/pr-comments.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1 # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/pr-comments.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/pr-comments.git +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
Fetching without tags
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/pr-comments.git # timeout=10
 > git config --add remote.origin.fetch +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/pr-comments.git # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/pr-comments.git
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/pr-comments.git +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
Checking out Revision 565d84f4e86c6c446b37591d4f820e1425f28e0a (PR-1)
Commit message: "Coverity PR Test"
First time build. Skipping changelog.
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 565d84f4e86c6c446b37591d4f820e1425f28e0a # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Coverity_Pr_Comments/PR-1
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm
[Pipeline] {
[Pipeline] sh
+ node --version
v22.16.0
[Pipeline] sh
+ npm --version
10.9.2
[Pipeline] sh
+ npm install
npm warn deprecated fsevents@1.2.9: fsevents 1 will break on node v14+ and could be using insecure binaries. Upgrade to fsevents 2.
npm warn deprecated set-value@2.0.0: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated mixin-deep@1.3.1: Critical bug fixed in v2.0.1, please upgrade to the latest version.
npm warn deprecated ini@1.3.5: Please update to ini >=1.3.6 to avoid a prototype pollution issue
npm warn deprecated set-value@0.4.3: Critical bug fixed in v3.0.1, please upgrade to the latest version.
npm warn deprecated path-is-absolute@2.0.0: This package is no longer relevant as Node.js 0.12 is unmaintained.
npm warn deprecated urix@0.1.0: Please see https://github.com/lydell/urix#deprecated
npm warn deprecated har-validator@5.1.3: this library is no longer supported
npm warn deprecated to-iso-string@0.0.2: to-iso-string has been deprecated, use @segment/to-iso-string instead.
npm warn deprecated cryptiles@2.0.5: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated resolve-url@0.2.1: https://github.com/lydell/resolve-url#deprecated
npm warn deprecated bcrypt-nodejs@0.0.3: bcrypt-nodejs is no longer actively maintained. Please use bcrypt or bcryptjs. See https://github.com/kelektiv/node.bcrypt.js/wiki/bcrypt-vs-brypt.js to learn more about these two options
npm warn deprecated cryptiles@0.2.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated source-map-url@0.4.0: See https://github.com/lydell/source-map-url#deprecated
npm warn deprecated boom@0.4.2: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated debug@3.2.6: Debug versions >=3.2.0 <3.2.7 || >=4 <4.3.1 have a low-severity ReDos regression when used in a Node.js environment. It is recommended you upgrade to 3.2.7 or 4.3.1. (https://github.com/visionmedia/debug/issues/797)
npm warn deprecated boom@2.10.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated chokidar@2.1.6: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@0.2.4: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated minimatch@0.3.0: Please update to minimatch 3.0.2 or higher to avoid a RegExp DoS issue
npm warn deprecated chokidar@2.1.8: Chokidar 2 does not receive security updates since 2019. Upgrade to chokidar 3 with 15x fewer dependencies
npm warn deprecated sntp@1.0.9: This module moved to @hapi/sntp. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated querystring@0.2.0: The querystring API is considered Legacy. new code should use the URLSearchParams API instead.
npm warn deprecated request@2.36.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated mkdirp@0.3.0: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated tough-cookie@2.2.2: ReDoS vulnerability parsing Set-Cookie https://nodesecurity.io/advisories/130
npm warn deprecated hoek@0.9.1: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated node-uuid@1.4.8: Use uuid module instead
npm warn deprecated uuid@3.3.2: Please upgrade  to version 7 or higher.  Older versions may use Math.random() in certain circumstances, which is known to be problematic.  See https://v8.dev/blog/math-random for details.
npm warn deprecated source-map-resolve@0.5.2: See https://github.com/lydell/source-map-resolve#deprecated
npm warn deprecated har-validator@2.0.6: this library is no longer supported
npm warn deprecated mkdirp@0.5.1: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)
npm warn deprecated hoek@2.16.3: This version has been deprecated in accordance with the hapi support policy (hapi.im/support). Please upgrade to the latest version to get the best features, bug fixes, and security patches. If you are unable to upgrade at this time, paid support is available for older versions (hapi.im/commercial).
npm warn deprecated request@2.79.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.88.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated request@2.67.0: request has been deprecated, see https://github.com/request/request/issues/3142
npm warn deprecated readdir-scoped-modules@1.0.2: This functionality has been moved to @npmcli/fs
npm warn deprecated hawk@1.0.0: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated hawk@3.1.3: This module moved to @hapi/hawk. Please make sure to switch over as this distribution is no longer supported and may contain bugs and critical security issues.
npm warn deprecated jade@0.26.3: Jade has been renamed to pug, please install the latest version of pug instead of jade
npm warn deprecated swig@1.4.2: This package is no longer maintained
npm warn deprecated bson@1.0.9: Fixed a critical issue with BSON serialization documented in CVE-2019-2391, see https://bit.ly/2KcpXdo for more details
npm warn deprecated nodeunit@0.9.5: you are strongly encouraged to use other testing options

added 962 packages, and audited 1412 packages in 20s

32 packages are looking for funding
  run `npm fund` for details

136 vulnerabilities (9 low, 35 moderate, 57 high, 35 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues possible (including breaking changes), run:
  npm audit fix --force

Some issues need review, and may require choosing
a different dependency.

Run `npm audit` for details.
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (coverity-pr-comments)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Pr_Comments
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [COVERITY]
[Security Scan] INFO: Parameters for coverity:
[Security Scan] INFO:  --- coverity_passphrase = ******************************************************************************
[Security Scan] INFO:  --- coverity_waitForScan = true
[Security Scan] INFO:  --- coverity_prComment_enabled = true
[Security Scan] INFO:  --- coverity_url = https://integrations-qa.dev.cnc.duckutil.net
[Security Scan] INFO:  --- coverity_prComment_impacts = HIGH,MEDIUM,
[Security Scan] INFO:  --- coverity_user = admin
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_ssl_trustAll = false
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Coverity parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Pr_Comments
[Security Scan] INFO: Github repositoryName: pr-comments
[Security Scan] INFO: Github repositoryOwner: coverity-cnc-jenkins-samples
[Security Scan] INFO: Github projectRepositoryPullNumber: 1
[Security Scan] INFO: Github branchName: PR-1
[Security Scan] INFO: Github githubHostUrl: https://github.com/
[Security Scan] INFO: Coverity Project Name: pr-comments
[Security Scan] INFO: Coverity Stream Name: pr-comments-main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Pr_Comments
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/coverity_input7960106081596276929.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 21:49:21.5000 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 21:49:21.5259 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 21:49:21.5925 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 21:49:21.5926 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 21:49:21.5926 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:49:21.5926 IST [Bridge CLI] INFO: coverity.connect.project.name = pr-comments [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5926 IST [Bridge CLI] INFO: coverity.connect.stream.name = pr-comments-main [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5926 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: coverity.prComment.enabled = true [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: coverity.prComment.impacts = [HIGH MEDIUM] [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: github.repository.branch.name = PR-1 [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: github.repository.name = pr-comments [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5927 IST [Bridge CLI] INFO: github.repository.owner.name = coverity-cnc-jenkins-samples [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5928 IST [Bridge CLI] INFO: github.repository.pull.number = 1 [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5928 IST [Bridge CLI] INFO: github.user.token = ***************************************** [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5928 IST [Bridge CLI] INFO: network.airgap = false [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5928 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input7960106081596276929.json]
2025-11-13 21:49:21.5928 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:49:21.5928 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 21:49:21.5931 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 21:49:21.5977 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 21:49:21.6421 IST [Check pull request] INFO: Pipeline triggered for Jenkins Pull request event
2025-11-13 21:49:21.6450 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 21:49:21.6451 IST [Check pull request] INFO: Adapter finished
2025-11-13 21:49:24.2149 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 21:49:24.3023 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 21:49:24.3024 IST [Bridge CLI] INFO: Starting adapters for stage connect-results-fetcher
2025-11-13 21:49:24.3024 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 21:49:24.3024 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 21:49:24.3029 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 21:49:24.3028 IST [Bridge CLI] INFO: Starting Adapter: Coverity Results
2025-11-13 21:49:24.3028 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 21:49:24.3033 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 21:49:24.3084 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 21:49:24.3085 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 21:49:24.3085 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 21:49:24.3864 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 21:49:24.3866 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=pr-comments-main -o commit.connect.project=pr-comments -o commit.connect.comparison-only=true -o commit.local.format=json -o commit.local.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json
2025-11-13 21:49:24.4412 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 21:49:24.4426 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 21:49:24.4426 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 21:49:24.4426 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 21:49:24.4426 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 21:49:24.4426 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 21:49:24.4452 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 21:49:24.4452 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 21:49:24.4465 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir create
2025-11-13 21:49:26.3156 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 21:49:29.4875 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 21:49:30.4012 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 21:49:31.7887 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 21:49:32.3112 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:49:32.3299 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 21:49:32.7978 IST [Coverity Connect Scan] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir'
2025-11-13 21:49:32.7980 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 21:49:33.1156 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 21:49:33.3720 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 21:49:33.6223 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 21:49:33.8725 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 21:49:34.1197 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 21:49:34.3641 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 21:49:34.6093 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 21:49:34.8484 IST [Coverity Connect Scan] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 21:49:34.8484 IST [Coverity Connect Scan] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 21:49:34.8484 IST [Coverity Connect Scan] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 21:49:34.8536 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 21:49:35.0920 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 21:49:35.3345 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 21:49:35.5873 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 21:49:35.8499 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 21:49:36.1160 IST [Coverity Connect Scan] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 21:49:36.1293 IST [Coverity Connect Scan] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 21:49:36.1293 IST [Coverity Connect Scan] INFO:           and it will not be updated.
2025-11-13 21:49:36.7697 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 21:49:37.2580 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 21:49:37.8773 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-988369288 --record-with-source
2025-11-13 21:49:37.8993 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 21:49:37.9137 IST [Coverity Connect Scan] INFO: Emitting 86 Files.
2025-11-13 21:49:38.3731 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 21:49:38.3834 IST [Coverity Connect Scan] INFO: Executing action No unwanted TUs to delete
2025-11-13 21:49:38.3835 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 21:49:38.3836 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 21:49:38.3838 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:49:38.4064 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 21:49:38.9245 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:49:38.9799 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 21:49:38.9799 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 86
2025-11-13 21:49:38.9799 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 21:49:38.9799 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 21:49:38.9799 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 21:49:38.9800 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 86
2025-11-13 21:49:38.9800 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32745
2025-11-13 21:49:38.9821 IST [Coverity Connect Scan] INFO: Capture phase took 7.194s.
2025-11-13 21:49:38.9822 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 21:49:38.9845 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 21:49:38.9854 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 21:49:39.3041 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 21:49:39.3636 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 21:49:39.3637 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 21:49:40.0615 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:49:45.5118 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:49:45.5119 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 21:49:45.5120 IST [Coverity Connect Scan] INFO: The scan ID is '8333ef8d-b82d-4774-a336-903a7b2a70aa'
2025-11-13 21:49:45.5125 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 21:49:45.5125 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:52:40.3929 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:52:43.0871 IST [Coverity Connect Scan] INFO: Comparison report written to file '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json'.
2025-11-13 21:52:43.0873 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 21:52:43.0873 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    4 issue(s)
2025-11-13 21:52:43.0874 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 21:52:43.0874 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    32 issue(s)
2025-11-13 21:52:43.0874 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 21:52:43.0874 IST [Coverity Connect Scan] INFO: Results are available at /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json
2025-11-13 21:52:43.0883 IST [Coverity Connect Scan] INFO: Analyze phase took 3m4.1s.
2025-11-13 21:52:43.0930 IST [Coverity Connect Scan] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 21:52:43.0930 IST [Coverity Connect Scan] WARNING: 
2025-11-13 21:52:43.0931 IST [Coverity Connect Scan] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 21:52:43.0931 IST [Coverity Connect Scan] WARNING:   * C#
2025-11-13 21:52:43.0931 IST [Coverity Connect Scan] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 21:52:43.0932 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 21:52:43.1052 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 21:52:43.1218 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 21:52:43.1219 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 21:52:43.1220 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.connect.results.comparison.path'
2025-11-13 21:52:43.1226 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 21:52:46.2454 IST [Coverity Results] INFO: Reading from Coverity Comparison file(new): /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json
2025-11-13 21:52:46.2524 IST [Coverity Results] WARNING: Found 2 Coverity issues to comment on, breaking the build
2025-11-13 21:52:46.2607 IST [Coverity Results] INFO: Provided value for resource 'bridge.break'
2025-11-13 21:52:46.2608 IST [Coverity Results] INFO: Added entry to resource 'commenter.issues'
2025-11-13 21:52:46.2609 IST [Coverity Results] INFO: Provided value for resource 'commenter.test.CoveritySAST.resultFetcher.successful'
2025-11-13 21:52:46.2610 IST [Coverity Results] INFO: Adapter finished
2025-11-13 21:52:46.2893 IST [Bridge CLI] INFO: Starting adapters for stage githubprcomment
2025-11-13 21:52:46.2893 IST [Bridge CLI] INFO: Starting Adapter: GitHub Commenter
2025-11-13 21:52:46.2895 IST [SCM Checker] INFO: Adapter finished
2025-11-13 21:52:46.6134 IST [GitHub Commenter] INFO: will use default GitHub API URL "https://api.github.com", as "github.api.url" and "github.host.url" is not configured
2025-11-13 21:52:49.3762 IST [GitHub Commenter] INFO: Adapter finished
2025-11-13 21:52:49.3882 IST [Bridge CLI] WARNING: Breaking the build as 'bridge.break' has been set to true
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Issue count not found in output file
[Security Scan] ERROR: Workflow failed! Exit code 8: The config option 'bridge.break' has been set to true
**************************** END EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Pipeline] }
[Pipeline] // dir
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (Declarative: Post Actions)
[Pipeline] echo
Black Duck Logs Publisher - Starting log upload process
[Pipeline] echo
Configuration: [githubOrg:coverity-cnc-jenkins-samples, repoName:pr-comments, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Coverity_Pr_Comments/PR-1
[Pipeline] echo
Build Number: 1
[Pipeline] echo
GitHub Organization: coverity-cnc-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: pr-comments
[Pipeline] echo
Target repository: coverity-cnc-jenkins-samples/pr-comments
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*