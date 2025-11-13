# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Pr_Comments/main`
- **Build Number:** #3
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 3 min 58 sec and counting
- **Timestamp:** 2025-11-13 21:52:41 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 7f85efbe18f60217a7be64eb7963519b2b220bcf
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/Github_Coverity_Pr_Comments_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
Fetching changes from the remote Git repository
 > git config remote.origin.url https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Fetching without tags
Fetching upstream changes from https://github.com/integrations-garage/blackduck-logs-publisher
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/integrations-garage/blackduck-logs-publisher +refs/heads/*:refs/remotes/origin/* # timeout=10
Checking out Revision e969196a63b1be83b84541b022f7aa52928bd5e5 (main)
 > git config core.sparsecheckout # timeout=10
 > git checkout -f e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
Commit message: "Phase 3 - 2"
 > git rev-list --no-walk e969196a63b1be83b84541b022f7aa52928bd5e5 # timeout=10
[Pipeline] Start of Pipeline
[Pipeline] node
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/.git # timeout=10
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/pr-comments.git # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/pr-comments.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/pr-comments.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Checking out Revision 7f85efbe18f60217a7be64eb7963519b2b220bcf (main)
Commit message: "Jenkins log upload - Build #2"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 7f85efbe18f60217a7be64eb7963519b2b220bcf # timeout=10
 > git rev-list --no-walk 6b705c131bf63aec94e9f7b630719d81d9a2848e # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Build)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
JOB_NAME: MBP_Github_Coverity_Pr_Comments/main
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm
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

up to date, audited 1412 packages in 21s

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
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm
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
[Security Scan] INFO: Coverity Project Name: pr-comments
[Security Scan] INFO: Coverity Stream Name: pr-comments-main
[Security Scan] INFO: Coverity PR Comment is ignored for non pull request scan
[Security Scan] INFO: Jenkins Job name: MBP_Github_Coverity_Pr_Comments
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/coverity_input9049824890493443057.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 21:49:23.4312 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 21:49:23.4425 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 21:49:23.5330 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 21:49:23.5331 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 21:49:23.5331 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:49:23.5331 IST [Bridge CLI] INFO: coverity.connect.project.name = pr-comments [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5332 IST [Bridge CLI] INFO: coverity.connect.stream.name = pr-comments-main [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5332 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5332 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5332 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5332 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5333 IST [Bridge CLI] INFO: network.airgap = false [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5333 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input9049824890493443057.json]
2025-11-13 21:49:23.5333 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:49:23.5333 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 21:49:23.5337 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 21:49:23.5387 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 21:49:23.5617 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 21:49:23.5619 IST [Check pull request] INFO: Adapter finished
2025-11-13 21:49:25.8553 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 21:49:25.9063 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 21:49:25.9064 IST [Bridge CLI] INFO: Starting adapters for stage connect-post-processing
2025-11-13 21:49:25.9064 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 21:49:25.9064 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 21:49:25.9068 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 21:49:25.9068 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Post Scan
2025-11-13 21:49:25.9068 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 21:49:25.9070 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 21:49:25.9116 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 21:49:25.9118 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 21:49:25.9118 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 21:49:25.9840 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 21:49:25.9841 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=pr-comments-main -o commit.connect.project=pr-comments
2025-11-13 21:49:26.0512 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 21:49:26.0537 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 21:49:26.0537 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 21:49:26.0537 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 21:49:26.0537 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 21:49:26.0538 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 21:49:26.0559 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir reset-host-name
2025-11-13 21:49:26.0756 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir check-compatible
2025-11-13 21:49:26.0989 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 21:49:26.0990 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 21:49:27.8823 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 21:49:31.0578 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 21:49:31.8314 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 21:49:33.1907 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 21:49:33.9130 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:49:33.9364 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 21:49:34.4311 IST [Coverity Connect Scan] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 21:49:34.9424 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 21:49:35.4245 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 21:49:36.1621 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-1229743902 --record-with-source
2025-11-13 21:49:36.2031 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 21:49:36.2239 IST [Coverity Connect Scan] INFO: Emitting 84 Files.
2025-11-13 21:49:36.4896 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 21:49:36.4924 IST [Coverity Connect Scan] INFO: Executing action No unwanted TUs to delete
2025-11-13 21:49:36.4924 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 21:49:36.4925 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 21:49:36.4927 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:49:36.5111 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 21:49:37.0652 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 21:49:37.1267 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 21:49:37.1268 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 84
2025-11-13 21:49:37.1268 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 21:49:37.1268 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 21:49:37.1268 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 21:49:37.1268 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 84
2025-11-13 21:49:37.1268 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32728
2025-11-13 21:49:37.1322 IST [Coverity Connect Scan] INFO: Capture phase took 3.942s.
2025-11-13 21:49:37.1322 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 21:49:37.1366 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_main/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 21:49:37.1385 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 21:49:37.4398 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 21:49:37.4831 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 21:49:37.4831 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 21:49:38.1877 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:49:43.9071 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:49:43.9072 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 21:49:43.9074 IST [Coverity Connect Scan] INFO: The scan ID is 'da1208fc-ce20-4342-a2e7-85d968e84b7e'
2025-11-13 21:49:43.9093 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 21:49:43.9094 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 21:52:38.0699 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 21:52:38.7603 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 21:52:38.7604 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    2 issue(s)
2025-11-13 21:52:38.7604 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 21:52:38.7604 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    25 issue(s)
2025-11-13 21:52:38.7605 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 21:52:38.7605 IST [Coverity Connect Scan] INFO: Results are available at https://integrations-qa.dev.cnc.duckutil.net:443/query/defects.htm?stream=pr-comments-main&outstanding=true
2025-11-13 21:52:38.7610 IST [Coverity Connect Scan] INFO: Analyze phase took 3m1.621s.
2025-11-13 21:52:38.7627 IST [Coverity Connect Scan] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 21:52:38.7627 IST [Coverity Connect Scan] WARNING: 
2025-11-13 21:52:38.7628 IST [Coverity Connect Scan] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 21:52:38.7628 IST [Coverity Connect Scan] WARNING:   * C#
2025-11-13 21:52:38.7630 IST [Coverity Connect Scan] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 21:52:38.7630 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 21:52:38.7662 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 21:52:38.7732 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 21:52:38.7734 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 21:52:38.7758 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 21:52:38.9319 IST [SCM Checker] INFO: Adapter finished
2025-11-13 21:52:40.6019 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.resultURL'
2025-11-13 21:52:40.6022 IST [Coverity Connect Post Scan] INFO: Provided value for resource 'coverity.connect.policy.issueCount'
2025-11-13 21:52:40.6030 IST [Coverity Connect Post Scan] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 39
[Security Scan] INFO: Security Scan execution is successful
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
Job Name: MBP_Github_Coverity_Pr_Comments/main
[Pipeline] echo
Build Number: 3
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