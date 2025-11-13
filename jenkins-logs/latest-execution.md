# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Coverity_Pr_Comments/PR-1`
- **Build Number:** #2
- **Build Status:** 🔴 **FAILURE**
- **Duration:** 2 min 48 sec and counting
- **Timestamp:** 2025-11-13 22:02:07 UTC

---

## Console Output

```
Started by user admin
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from 2c12ca221e004425dff1580be5e36ecf5e326671
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/Github_Coverity_Pr_Comments_PR-1@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Fetching changes from the remote Git repository
Fetching without tags
 > git rev-parse --resolve-git-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/.git # timeout=10
 > git config remote.origin.url https://github.com/coverity-cnc-jenkins-samples/pr-comments.git # timeout=10
Fetching upstream changes from https://github.com/coverity-cnc-jenkins-samples/pr-comments.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/coverity-cnc-jenkins-samples/pr-comments.git +refs/pull/1/head:refs/remotes/origin/PR-1 # timeout=10
Checking out Revision 2c12ca221e004425dff1580be5e36ecf5e326671 (PR-1)
Commit message: "Coverity PR Comments Test"
 > git config core.sparsecheckout # timeout=10
 > git checkout -f 2c12ca221e004425dff1580be5e36ecf5e326671 # timeout=10
 > git rev-list --no-walk 565d84f4e86c6c446b37591d4f820e1425f28e0a # timeout=10
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
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage connect --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/coverity_input14328027679327972157.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 21:59:58.4981 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 21:59:58.5083 IST [Bridge CLI] INFO: Found version "3.0.128" in registry for workflow "connect", trying to load it from local cache
2025-11-13 21:59:58.5889 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.connect.project.name = pr-comments [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.connect.stream.name = pr-comments-main [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.connect.url = https://integrations-qa.dev.cnc.duckutil.net [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.connect.user.name = admin [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.connect.user.password = ***************************************** [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.prComment.enabled = true [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: coverity.waitForScan = true [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5890 IST [Bridge CLI] INFO: github.repository.branch.name = PR-1 [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: github.repository.name = pr-comments [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: github.repository.owner.name = coverity-cnc-jenkins-samples [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: github.repository.pull.number = 1 [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: github.user.token = ***************************************** [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: network.airgap = false [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: network.ssl.trustAll = false [coverity_input14328027679327972157.json]
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 21:59:58.5891 IST [Bridge CLI] INFO: Starting adapters for stage connect
2025-11-13 21:59:58.5894 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Controller
2025-11-13 21:59:58.5938 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 21:59:58.6198 IST [Check pull request] INFO: Pipeline triggered for Jenkins Pull request event
2025-11-13 21:59:58.6223 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 21:59:58.6225 IST [Check pull request] INFO: Adapter finished
2025-11-13 22:00:01.2334 IST [Coverity Connect Controller] INFO: No coverity version is configured, will use the default or latest supported version from the server
2025-11-13 22:00:01.3226 IST [Coverity Connect Controller] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 22:00:01.3226 IST [Bridge CLI] INFO: Starting adapters for stage connect-results-fetcher
2025-11-13 22:00:01.3226 IST [Bridge CLI] INFO: Starting adapters for stage scm
2025-11-13 22:00:01.3226 IST [Bridge CLI] INFO: Starting adapters for stage connect-scan
2025-11-13 22:00:01.3235 IST [Bridge CLI] INFO: Starting Adapter: Coverity Connect Scan
2025-11-13 22:00:01.3235 IST [Bridge CLI] INFO: Starting Adapter: Coverity Results
2025-11-13 22:00:01.3235 IST [Bridge CLI] INFO: Starting Adapter: SCM Checker
2025-11-13 22:00:01.3238 IST [Coverity Connect Controller] INFO: Adapter finished
2025-11-13 22:00:01.3281 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for Set Version for Coverity
2025-11-13 22:00:01.3282 IST [Default Adapter for Set Version for Coverity] INFO: Provided value for resource 'coverity.version'
2025-11-13 22:00:01.3283 IST [Default Adapter for Set Version for Coverity] INFO: Adapter finished
2025-11-13 22:00:01.4002 IST [Coverity Connect Scan] INFO: Identified workflow: Coverity
2025-11-13 22:00:01.4007 IST [Coverity Connect Scan] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity scan --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -o analyze.location=connect -o commit.connect.url=https://integrations-qa.dev.cnc.duckutil.net -o commit.connect.stream=pr-comments-main -o commit.connect.project=pr-comments -o commit.connect.comparison-only=true -o commit.local.format=json -o commit.local.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json
2025-11-13 22:00:01.4647 IST [Coverity Connect Scan] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 22:00:01.4695 IST [Coverity Connect Scan] WARNING: No setting for 'commit.connect.on-new-cert' specified.
2025-11-13 22:00:01.4695 IST [Coverity Connect Scan] WARNING: Using default value of 'distrust'.
2025-11-13 22:00:01.4695 IST [Coverity Connect Scan] WARNING: This may result in a certificate validation error when uploading defects to Coverity Connect.
2025-11-13 22:00:01.4695 IST [Coverity Connect Scan] WARNING: If you trust the Coverity Connect instance and certificate validation fails, set 'commit.connect.on-new-cert' to 'trust'.
2025-11-13 22:00:01.4696 IST [Coverity Connect Scan] WARNING: If you are unfamiliar with what this means, please talk to your Coverity Connect administrator.
2025-11-13 22:00:01.4738 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir reset-host-name
2025-11-13 22:00:01.5283 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir check-compatible
2025-11-13 22:00:01.5532 IST [Coverity Connect Scan] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 22:00:01.5533 IST [Coverity Connect Scan] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 22:00:03.3630 IST [Coverity Connect Scan] INFO: Cloud analysis is enabled.
2025-11-13 22:00:06.6847 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 22:00:07.6286 IST [Coverity Connect Scan] INFO: Caching is enabled.
2025-11-13 22:00:09.1055 IST [Coverity Connect Scan] INFO: Telemetry is enabled
2025-11-13 22:00:09.7084 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 22:00:09.7336 IST [Coverity Connect Scan] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 22:00:10.1671 IST [Coverity Connect Scan] INFO: Executing action no-op: skipping compiler configuration
2025-11-13 22:00:10.5979 IST [Coverity Connect Scan] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 22:00:11.0089 IST [Coverity Connect Scan] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 22:00:11.5526 IST [Coverity Connect Scan] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/capture-file-list-1577197692 --record-with-source
2025-11-13 22:00:11.5817 IST [Coverity Connect Scan] INFO: Buildless capture started.
2025-11-13 22:00:11.6001 IST [Coverity Connect Scan] INFO: Emitting 87 Files.
2025-11-13 22:00:11.7936 IST [Coverity Connect Scan] INFO: Buildless capture completed.
2025-11-13 22:00:11.7959 IST [Coverity Connect Scan] INFO: Executing action No unwanted TUs to delete
2025-11-13 22:00:11.7960 IST [Coverity Connect Scan] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 22:00:11.7960 IST [Coverity Connect Scan] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir
2025-11-13 22:00:11.7963 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 22:00:11.8250 IST [Coverity Connect Scan] INFO: Executing action Invalidate capture results
2025-11-13 22:00:12.3145 IST [Coverity Connect Scan] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir list-capture-diagnostics
2025-11-13 22:00:12.3685 IST [Coverity Connect Scan] INFO: Capture summary:
2025-11-13 22:00:12.3685 IST [Coverity Connect Scan] INFO:     SUCCEEDED: 87
2025-11-13 22:00:12.3685 IST [Coverity Connect Scan] INFO:     INCOMPLETE: 0
2025-11-13 22:00:12.3685 IST [Coverity Connect Scan] INFO:     FAILED: 0
2025-11-13 22:00:12.3686 IST [Coverity Connect Scan] INFO:     IGNORED: 6
2025-11-13 22:00:12.3686 IST [Coverity Connect Scan] INFO:     FILES CAPTURED: 87
2025-11-13 22:00:12.3686 IST [Coverity Connect Scan] INFO:     LINES OF CODE: 32760
2025-11-13 22:00:12.3720 IST [Coverity Connect Scan] INFO: Capture phase took 3.27s.
2025-11-13 22:00:12.3721 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml'
2025-11-13 22:00:12.3744 IST [Coverity Connect Scan] INFO: Loading compiler config '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml'
2025-11-13 22:00:12.3755 IST [Coverity Connect Scan] INFO: Analyzing project in the cloud using Coverity Analysis version 2025.9.0
2025-11-13 22:00:12.6761 IST [Coverity Connect Scan] INFO: Creating archive containing data to be analyzed...
2025-11-13 22:00:12.7357 IST [Coverity Connect Scan] INFO: Properties archive created.
2025-11-13 22:00:12.7358 IST [Coverity Connect Scan] INFO: Uploading data for analysis...
2025-11-13 22:00:13.4580 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 22:00:19.2418 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 22:00:19.2422 IST [Coverity Connect Scan] INFO: Scan created.
2025-11-13 22:00:19.2423 IST [Coverity Connect Scan] INFO: The scan ID is 'cf371d63-1cc1-470f-b89a-5d128f4c183b'
2025-11-13 22:00:19.2432 IST [Coverity Connect Scan] INFO: Waiting for scan to complete...
2025-11-13 22:00:19.2432 IST [Coverity Connect Scan] INFO: |0----------25-----------50----------75---------100|
2025-11-13 22:02:01.2700 IST [Coverity Connect Scan] INFO: ****************************************************
2025-11-13 22:02:03.9391 IST [Coverity Connect Scan] INFO: Comparison report written to file '/Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json'.
2025-11-13 22:02:03.9408 IST [Coverity Connect Scan] INFO: Analysis summary after merging defects:
2025-11-13 22:02:03.9408 IST [Coverity Connect Scan] INFO:     HIGH SEVERITY:    6 issue(s)
2025-11-13 22:02:03.9408 IST [Coverity Connect Scan] INFO:     MEDIUM SEVERITY: 12 issue(s)
2025-11-13 22:02:03.9409 IST [Coverity Connect Scan] INFO:     LOW SEVERITY:    38 issue(s)
2025-11-13 22:02:03.9409 IST [Coverity Connect Scan] INFO:     AUDIT SEVERITY:   0 issue(s)
2025-11-13 22:02:03.9409 IST [Coverity Connect Scan] INFO: Results are available at /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json
2025-11-13 22:02:03.9437 IST [Coverity Connect Scan] INFO: Analyze phase took 1m51.566s.
2025-11-13 22:02:03.9447 IST [Coverity Connect Scan] WARNING: !! SOURCES FOR UNSUPPORTED LANGUAGES WERE DETECTED !!
2025-11-13 22:02:03.9448 IST [Coverity Connect Scan] WARNING: 
2025-11-13 22:02:03.9448 IST [Coverity Connect Scan] WARNING: Source files for the following languages were detected, but these languages are not supported on Mac OS ARM:
2025-11-13 22:02:03.9448 IST [Coverity Connect Scan] WARNING:   * C#
2025-11-13 22:02:03.9449 IST [Coverity Connect Scan] WARNING: In order to analyze these files, please analyze the project on an operating system and architecture where they are supported.
2025-11-13 22:02:03.9449 IST [Coverity Connect Scan] INFO: Scan complete.
2025-11-13 22:02:03.9506 IST [Coverity Connect Scan] INFO: Coverity Capture completed successfully
2025-11-13 22:02:03.9598 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.completed'
2025-11-13 22:02:03.9600 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 22:02:03.9602 IST [Coverity Connect Scan] INFO: Provided value for resource 'coverity.connect.results.comparison.path'
2025-11-13 22:02:03.9608 IST [Coverity Connect Scan] INFO: Adapter finished
2025-11-13 22:02:03.9960 IST [Coverity Results] INFO: Reading from Coverity Comparison file(new): /Users/madhusud/Jenkins_Testing/Nodes/workspace/Github_Coverity_Pr_Comments_PR-1/nodejs-npm/.bridge/coverity_connect_scan/comparison-report/report.json
2025-11-13 22:02:03.9979 IST [Coverity Results] INFO: No impacts set for Coverity PR comment, using default impacts: [High]
2025-11-13 22:02:03.9979 IST [Coverity Results] WARNING: Found 4 Coverity issues to comment on, breaking the build
2025-11-13 22:02:04.0009 IST [Coverity Results] INFO: Provided value for resource 'bridge.break'
2025-11-13 22:02:04.0010 IST [Coverity Results] INFO: Added entry to resource 'commenter.issues'
2025-11-13 22:02:04.0012 IST [Coverity Results] INFO: Provided value for resource 'commenter.test.CoveritySAST.resultFetcher.successful'
2025-11-13 22:02:04.0014 IST [Coverity Results] INFO: Adapter finished
2025-11-13 22:02:04.0488 IST [Bridge CLI] INFO: Starting adapters for stage githubprcomment
2025-11-13 22:02:04.0489 IST [Bridge CLI] INFO: Starting Adapter: GitHub Commenter
2025-11-13 22:02:04.0490 IST [SCM Checker] INFO: Adapter finished
2025-11-13 22:02:04.0911 IST [GitHub Commenter] INFO: will use default GitHub API URL "https://api.github.com", as "github.api.url" and "github.host.url" is not configured
2025-11-13 22:02:06.4934 IST [GitHub Commenter] INFO: Adapter finished
2025-11-13 22:02:06.5004 IST [Bridge CLI] WARNING: Breaking the build as 'bridge.break' has been set to true
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
Build Number: 2
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