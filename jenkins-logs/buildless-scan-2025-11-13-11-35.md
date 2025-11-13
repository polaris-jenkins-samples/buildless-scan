# Jenkins Execution Log

## Build Information
- **Job Name:** `MBP_Github_Polaris_Buildless_Scan/main`
- **Build Number:** #2
- **Build Status:** 🟢 **SUCCESS**
- **Duration:** 1 min 11 sec and counting
- **Timestamp:** 2025-11-13 11:35:40 UTC

---

## Console Output

```
Branch indexing
Connecting to https://api.github.com using madhusud@blackduck.com/****** (Github_Username_PAT)
Obtained nodejs-npm/Jenkinsfile from ff58d1f799e68044b728906a9387190ea0659875
Loading library blackduck-logs-publisher@main
Attempting to resolve main from remote references...
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git ls-remote -h -- https://github.com/integrations-garage/blackduck-logs-publisher # timeout=10
Found match: refs/heads/main revision e969196a63b1be83b84541b022f7aa52928bd5e5
The recommended git tool is: NONE
using credential Github_Username_PAT
 > git rev-parse --resolve-git-dir /Users/madhusud/.jenkins/workspace/thub_Polaris_Buildless_Scan_main@libs/a0dda568bac7bbb4a171f59ba3f2660c21c69edc6356524e9ae8bb4500c12bbb/.git # timeout=10
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
Running on mac-sh in /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2
[Pipeline] {
[Pipeline] stage
[Pipeline] { (Declarative: Checkout SCM)
[Pipeline] checkout
The recommended git tool is: NONE
using credential Github_Username_PAT
Cloning the remote Git repository
Cloning with configured refspecs honoured and without tags
Cloning repository https://github.com/polaris-jenkins-samples/buildless-scan.git
 > git init /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2 # timeout=10
Fetching upstream changes from https://github.com/polaris-jenkins-samples/buildless-scan.git
 > git --version # timeout=10
 > git --version # 'git version 2.39.5 (Apple Git-154)'
using GIT_ASKPASS to set credentials Github_Username_PAT
 > git fetch --no-tags --force --progress -- https://github.com/polaris-jenkins-samples/buildless-scan.git +refs/heads/main:refs/remotes/origin/main # timeout=10
Avoid second fetch
Checking out Revision ff58d1f799e68044b728906a9387190ea0659875 (main)
Commit message: "Polaris Buildless Scan"
First time build. Skipping changelog.
 > git config remote.origin.url https://github.com/polaris-jenkins-samples/buildless-scan.git # timeout=10
 > git config --add remote.origin.fetch +refs/heads/main:refs/remotes/origin/main # timeout=10
 > git config core.sparsecheckout # timeout=10
 > git checkout -f ff58d1f799e68044b728906a9387190ea0659875 # timeout=10
[Pipeline] }
[Pipeline] // stage
[Pipeline] withEnv
[Pipeline] {
[Pipeline] stage
[Pipeline] { (polaris-buildless-scan)
[Pipeline] script
[Pipeline] {
[Pipeline] dir
Running in /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm
[Pipeline] {
[Pipeline] security_scan
**************************** START EXECUTION OF BLACK DUCK SECURITY SCAN ****************************
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Buildless_Scan
-------------------------------- Connection to node --------------------------------
[Security Scan] INFO: Jenkins job is running on agent node remotely
-------------------------- Parameter Validation Initiated --------------------------
[Security Scan] INFO:  --- product = [POLARIS]
[Security Scan] INFO: Parameters for polaris:
[Security Scan] INFO:  --- polaris_waitForScan = true
[Security Scan] INFO:  --- polaris_server_url = https://poc.polaris.blackduck.com
[Security Scan] INFO:  --- polaris_assessment_types = SAST,SCA
[Security Scan] INFO:  --- polaris_access_token = ******************************************************************************
------------------------------------------------------------------------------------
[Security Scan] INFO: Parameters for additional configuration:
[Security Scan] INFO:  --- network_airgap = false
[Security Scan] INFO: Polaris parameters are validated successfully
[Security Scan] INFO: Bridge download parameters are validated successfully
[Security Scan] INFO: Bridge download is not required. Found installed in: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
------------------------------------------------------------------------------------
[Security Scan] INFO: Bridge CLI version is - 3.9.2
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Buildless_Scan
[Security Scan] INFO: Polaris Application Name: buildless-scan
[Security Scan] INFO: Polaris Project Name: buildless-scan
[Security Scan] INFO: Polaris Branch Name: main
[Security Scan] INFO: Jenkins Job name: MBP_Github_Polaris_Buildless_Scan
[Security Scan] INFO: Executable command line arguments: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm/bridge-cli --stage polaris --input /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/polaris_input9003220048068304701.json --out .bridge/output/scan_info_out.json

******************************* START EXECUTION OF BRIDGE CLI *******************************
2025-11-13 11:34:38.3712 IST [Bridge CLI] INFO: Using cache directory: /Users/madhusud/bridge-cli-bundle/bridge-cli-bundle-macos_arm
2025-11-13 11:34:38.3779 IST [Bridge CLI] INFO: Found version "3.0.371" in registry for workflow "polaris", trying to load it from local cache
2025-11-13 11:34:39.7132 IST [Bridge CLI] INFO: Input Resources:
2025-11-13 11:34:39.7133 IST [Bridge CLI] INFO: resource = value [source]
2025-11-13 11:34:39.7133 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 11:34:39.7133 IST [Bridge CLI] INFO: network.airgap = false [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7133 IST [Bridge CLI] INFO: polaris.accesstoken = ***************************************** [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7133 IST [Bridge CLI] INFO: polaris.application.name = buildless-scan [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7133 IST [Bridge CLI] INFO: polaris.assessment.types = [SAST SCA] [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7134 IST [Bridge CLI] INFO: polaris.branch.name = main [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7134 IST [Bridge CLI] INFO: polaris.project.name = buildless-scan [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7134 IST [Bridge CLI] INFO: polaris.serverUrl = https://poc.polaris.blackduck.com [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7134 IST [Bridge CLI] INFO: polaris.waitForScan = true [polaris_input9003220048068304701.json]
2025-11-13 11:34:39.7134 IST [Bridge CLI] INFO: ------------------------------------------------------------
2025-11-13 11:34:39.7134 IST [Bridge CLI] INFO: Starting adapters for stage polaris
2025-11-13 11:34:39.7151 IST [Bridge CLI] INFO: Starting Adapter: Polaris Status Provider
2025-11-13 11:34:39.7151 IST [Bridge CLI] INFO: Starting Adapter: Polaris Initializer
2025-11-13 11:34:39.7151 IST [Bridge CLI] INFO: Starting Adapter: Polaris Controller
2025-11-13 11:34:39.7151 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCM Discovery
2025-11-13 11:34:39.7875 IST [Polaris SCM Discovery] INFO: Adapter finished
2025-11-13 11:34:39.7909 IST [Bridge CLI] INFO: Starting Adapter: Set Polaris Assessment Mode to CI
2025-11-13 11:34:39.7911 IST [Set Polaris Assessment Mode to CI] INFO: Provided value for resource 'polaris.assessment.mode'
2025-11-13 11:34:39.7911 IST [Set Polaris Assessment Mode to CI] INFO: Adapter finished
2025-11-13 11:34:39.7944 IST [Bridge CLI] INFO: Starting Adapter: Create Polaris Project & Branch By Default
2025-11-13 11:34:39.7945 IST [Create Polaris Project & Branch By Default] INFO: Provided value for resource 'polaris.onboarding'
2025-11-13 11:34:39.7945 IST [Create Polaris Project & Branch By Default] INFO: Adapter finished
2025-11-13 11:34:41.7083 IST [Polaris Initializer] INFO: Successfully created test for "SAST(sastFull)" assessment. The short test ID is "LY0HXDJ"
2025-11-13 11:34:41.7142 IST [Polaris Initializer] INFO: Successfully created test for "SCA(scaPackage)" assessment. The short test ID is "LIX7CLU"
2025-11-13 11:34:41.7377 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.id'
2025-11-13 11:34:41.7381 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.id'
2025-11-13 11:34:41.7384 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.shortId'
2025-11-13 11:34:41.7387 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.shortId'
2025-11-13 11:34:41.7391 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.streamId'
2025-11-13 11:34:41.7393 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.project.id'
2025-11-13 11:34:41.7396 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.branch.id'
2025-11-13 11:34:41.7399 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.portfolioid'
2025-11-13 11:34:41.7402 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.tenant.id'
2025-11-13 11:34:41.7404 IST [Polaris Initializer] INFO: Provided value for resource 'polaris.application.id'
2025-11-13 11:34:41.7410 IST [Polaris Initializer] INFO: Adapter finished
2025-11-13 11:34:41.7601 IST [Bridge CLI] INFO: Starting Adapter: Check pull request
2025-11-13 11:34:41.8098 IST [Check pull request] INFO: Provided value for resource 'environment.scan.pull'
2025-11-13 11:34:41.8101 IST [Check pull request] INFO: Adapter finished
2025-11-13 11:34:41.8555 IST [Polaris Controller] INFO: Running for "sast" assessment with scan type "sastFull"
2025-11-13 11:34:41.8557 IST [Polaris Controller] INFO: fetching recommended "coverity" tool info...
2025-11-13 11:34:42.1881 IST [Polaris Controller] INFO: checking "coverity" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0
2025-11-13 11:34:42.1881 IST [Polaris Controller] INFO: Checking tool version for "cov_thin_client" in "/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0"
2025-11-13 11:34:42.1883 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity --version
2025-11-13 11:34:42.2571 IST [Polaris Controller] INFO: Got tool version for "cov_thin_client": 2025.9.0
2025-11-13 11:34:42.5559 IST [Polaris Controller] INFO: "coverity" tool is already installed...
2025-11-13 11:34:42.5563 IST [Polaris Controller] INFO: fetching recommended "Sigma" tool info...
2025-11-13 11:34:42.8574 IST [Polaris Controller] INFO: checking "Sigma" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0
2025-11-13 11:34:42.8576 IST [Polaris Controller] INFO: Checking tool version for "sigma" in "/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0"
2025-11-13 11:34:42.8578 IST [Polaris Controller] INFO: Running command:/Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --version
2025-11-13 11:34:42.9382 IST [Polaris Controller] INFO: Got tool version for "sigma": 2025.10.0
2025-11-13 11:34:43.2437 IST [Polaris Controller] INFO: "Sigma" tool is already installed...
2025-11-13 11:34:43.2440 IST [Polaris Controller] INFO: Running for "sca" assessment with scan type "scaPackage"
2025-11-13 11:34:43.2440 IST [Polaris Controller] INFO: fetching recommended "detect" tool info...
2025-11-13 11:34:43.5451 IST [Polaris Controller] INFO: checking "detect" tool installation inside bridge home directory: /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0
2025-11-13 11:34:43.5454 IST [Polaris Controller] INFO: Running command:/Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -version
2025-11-13 11:34:43.6426 IST [Polaris Controller] INFO: Checking tool version for "detect" in "/Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0"
2025-11-13 11:34:43.6461 IST [Polaris Controller] INFO: Got tool version for "detect": 10.4.0
2025-11-13 11:34:43.9412 IST [Polaris Controller] INFO: "detect" tool is already installed...
2025-11-13 11:34:43.9685 IST [Polaris Controller] INFO: Provided value for resource 'coverity.id'
2025-11-13 11:34:43.9687 IST [Polaris Controller] INFO: Provided value for resource 'sigma.id'
2025-11-13 11:34:43.9689 IST [Polaris Controller] INFO: Provided value for resource 'detect.id'
2025-11-13 11:34:43.9690 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sast
2025-11-13 11:34:43.9690 IST [Bridge CLI] INFO: Starting adapters for stage polaris-sca-package
2025-11-13 11:34:43.9690 IST [Bridge CLI] INFO: Starting adapters for stage polaris-artifacts-uploader
2025-11-13 11:34:43.9690 IST [Bridge CLI] INFO: Starting adapters for stage polaris-post-processing
2025-11-13 11:34:43.9706 IST [Bridge CLI] INFO: Starting Adapter: Polaris SCA Package Manager Scan
2025-11-13 11:34:43.9706 IST [Bridge CLI] INFO: Starting Adapter: Polaris Coverity Capture
2025-11-13 11:34:43.9706 IST [Bridge CLI] INFO: Starting Adapter: Polaris Artifacts Uploader
2025-11-13 11:34:43.9707 IST [Bridge CLI] INFO: Starting Adapter: Polaris Waiter
2025-11-13 11:34:43.9712 IST [Polaris Controller] INFO: Adapter finished
2025-11-13 11:34:43.9707 IST [Bridge CLI] INFO: Starting Adapter: Polaris Issues Fetcher
2025-11-13 11:34:43.9708 IST [Bridge CLI] INFO: Starting Adapter: Polaris Policy Checker
2025-11-13 11:34:44.0077 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:34:44.0078 IST [Default Adapter for execution path] INFO: Provided value for resource 'coverity.execution.path'
2025-11-13 11:34:44.0079 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:34:44.0150 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:34:44.0151 IST [Default Adapter for execution path] INFO: Provided value for resource 'sigma.execution.path'
2025-11-13 11:34:44.0151 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:34:44.0748 IST [Polaris Coverity Capture] INFO: Identified workflow: Polaris
2025-11-13 11:34:44.0754 IST [Polaris Coverity Capture] INFO: command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity capture --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect
2025-11-13 11:34:44.1324 IST [Polaris Coverity Capture] INFO: coverity 2025.9.0 covcli-2025.9-push-12
2025-11-13 11:34:44.1325 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_API_TOKEN_FILE=/var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/polaris_coverity_cache2184671745/.authKey
2025-11-13 11:34:44.1325 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_KEY=faa44fe7-68f2-46e6-8afa-ab21b990e542
2025-11-13 11:34:44.1325 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CACHE_URL=https://poc.polaris.blackduck.com/api/cache
2025-11-13 11:34:44.1325 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_CAPTURE_ZIP_ARCHIVE=/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip
2025-11-13 11:34:44.1325 IST [Polaris Coverity Capture] INFO: envvar: COVERITY_CLI_POLARIS_CLIENT=true
2025-11-13 11:34:44.1335 IST [Polaris Coverity Capture] INFO: Detected that stdout is not connected to a terminal.  Defaulting ticker mode to 'none'.
2025-11-13 11:34:44.1335 IST [Polaris Coverity Capture] INFO: If this is not correct, explicitly set the ticker mode to the desired value using the '--ticker-mode' option.
2025-11-13 11:34:44.1345 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir create
2025-11-13 11:34:44.1808 IST [Polaris Coverity Capture] INFO: Using lightweight capture with thin client.
2025-11-13 11:34:44.1808 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-manage-cache check
2025-11-13 11:34:44.5777 IST [Polaris Coverity Capture] INFO: Caching is enabled.
2025-11-13 11:34:44.5811 IST [Polaris Coverity Capture] INFO: Telemetry is enabled
2025-11-13 11:34:44.5990 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:34:44.6374 IST [Polaris Coverity Capture] INFO: Executing action no-op: nothing to do for initialization
2025-11-13 11:34:44.6475 IST [Polaris Coverity Capture] INFO: Executing action Delete compiler configurations for intermediate directory '/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir'
2025-11-13 11:34:44.6477 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler gcc --comptype clangcc --template
2025-11-13 11:34:44.9308 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler cc --comptype gcc --template
2025-11-13 11:34:45.1830 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler c++ --comptype g++ --template
2025-11-13 11:34:45.4452 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler clang --comptype clangcc --template
2025-11-13 11:34:45.6737 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler java --comptype java --template
2025-11-13 11:34:45.9036 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler go --comptype go --template
2025-11-13 11:34:46.1465 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler ccache --comptype prefix --template
2025-11-13 11:34:46.3782 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/build-compiler-configs/coverity_config.xml --compiler kotlinc --comptype kotlinc --template
2025-11-13 11:34:46.6086 IST [Polaris Coverity Capture] WARNING: Template config template-java-config-0 already exists for java and will be reused. 
2025-11-13 11:34:46.6087 IST [Polaris Coverity Capture] WARNING: Template config template-apt-config-0 already exists for apt and will be reused. 
2025-11-13 11:34:46.6087 IST [Polaris Coverity Capture] WARNING: Template config template-javaw-config-0 already exists for javaw and will be reused. 
2025-11-13 11:34:46.6137 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --dart
2025-11-13 11:34:46.8344 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --javascript
2025-11-13 11:34:47.0584 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --php
2025-11-13 11:34:47.2883 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --python
2025-11-13 11:34:47.5170 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ruby
2025-11-13 11:34:47.7491 IST [Polaris Coverity Capture] INFO: Executing action Configure build compiler: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-configure -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --comptype capture-config-files --file-regex $capture-config-files$ --template
2025-11-13 11:34:47.7607 IST [Polaris Coverity Capture] WARNING: Configuration already exists for file regex $capture-config-files$
2025-11-13 11:34:47.7607 IST [Polaris Coverity Capture] INFO:           and it will not be updated.
2025-11-13 11:34:47.7680 IST [Polaris Coverity Capture] INFO: Executing action no-op: no compilers need to be unconfigured
2025-11-13 11:34:47.7738 IST [Polaris Coverity Capture] INFO: Executing action no-op: compiler configurations loaded
2025-11-13 11:34:47.7792 IST [Polaris Coverity Capture] INFO: Executing action Emit files using buildless capture: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-internal-capture-files --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -c /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/buildless-compiler-configs/coverity_config.xml --ticker-mode none --append-log --capture-list-file /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir/coverity-cli/capture-file-list-2604080941 --record-with-source
2025-11-13 11:34:47.8032 IST [Polaris Coverity Capture] INFO: Buildless capture started.
2025-11-13 11:34:47.8167 IST [Polaris Coverity Capture] INFO: Emitting 84 Files.
2025-11-13 11:34:48.2962 IST [Polaris Coverity Capture] INFO: Buildless capture completed.
2025-11-13 11:34:48.2980 IST [Polaris Coverity Capture] INFO: Executing action No unwanted TUs to delete
2025-11-13 11:34:48.2980 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Unwanted TUs action cleanup
2025-11-13 11:34:48.2981 IST [Polaris Coverity Capture] INFO: Executing action deleteResidualTUs /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir
2025-11-13 11:34:48.2983 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:34:48.3158 IST [Polaris Coverity Capture] INFO: Executing action Invalidate capture results
2025-11-13 11:34:48.3159 IST [Polaris Coverity Capture] INFO: Executing action Invoke cov-run-sigma: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-run-sigma --project-dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir --coverity-config /var/folders/wm/gkd75sk54h57yqd0_j95gp2r0000gn/T/cov-run-sigma-config-1755291651/coverity.yaml --sigma-binary-path /Users/madhusud/.blackduck/bridge/tools/sigma/2025.10.0/sigma --enable-telemetry
2025-11-13 11:34:48.3457 IST [Polaris Coverity Capture] INFO: cov-run-sigma version 2025.9.0 on Darwin 24.6.0 arm64
2025-11-13 11:34:48.3458 IST [Polaris Coverity Capture] INFO: Internal version numbers: 477d3c5ddd p-2025.9-push-57
2025-11-13 11:34:48.3458 IST [Polaris Coverity Capture] INFO: 
2025-11-13 11:34:49.8927 IST [Polaris Coverity Capture] INFO: Executing action Action cleanup: Coverity configuration for Sigma
2025-11-13 11:34:49.8977 IST [Polaris Coverity Capture] INFO: Executing command: /Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/cov-manage-emit --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir list-capture-diagnostics
2025-11-13 11:34:49.9158 IST [Polaris Coverity Capture] INFO: Capture summary:
2025-11-13 11:34:49.9158 IST [Polaris Coverity Capture] INFO:     SUCCEEDED: 87
2025-11-13 11:34:49.9158 IST [Polaris Coverity Capture] INFO:     INCOMPLETE: 0
2025-11-13 11:34:49.9159 IST [Polaris Coverity Capture] INFO:     FAILED: 0
2025-11-13 11:34:49.9159 IST [Polaris Coverity Capture] INFO:     IGNORED: 3
2025-11-13 11:34:49.9159 IST [Polaris Coverity Capture] INFO:     FILES CAPTURED: 87
2025-11-13 11:34:49.9159 IST [Polaris Coverity Capture] INFO:     LINES OF CODE: 32908
2025-11-13 11:34:49.9166 IST [Polaris Coverity Capture] INFO: Capture phase took 5.339s.
2025-11-13 11:34:49.9405 IST [Polaris Coverity Capture] INFO: To analyze your project, type '/Users/madhusud/.blackduck/bridge/tools/cov-thin-client/2025.9.0/bin/coverity analyze --dir /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/2025.9.0/idir -o analyze.location=connect'.
2025-11-13 11:34:49.9419 IST [Polaris Coverity Capture] INFO: Coverity Capture completed successfully
2025-11-13 11:34:49.9490 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.completed'
2025-11-13 11:34:49.9491 IST [Polaris Coverity Capture] INFO: Provided value for resource 'coverity.idir.output'
2025-11-13 11:34:49.9493 IST [Polaris Coverity Capture] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.path'
2025-11-13 11:34:49.9495 IST [Polaris Coverity Capture] INFO: Adapter finished
2025-11-13 11:34:49.9509 IST [Bridge CLI] INFO: Starting Adapter: Default Adapter for execution path
2025-11-13 11:34:49.9510 IST [Default Adapter for execution path] INFO: Provided value for resource 'detect.execution.path'
2025-11-13 11:34:49.9511 IST [Default Adapter for execution path] INFO: Adapter finished
2025-11-13 11:34:49.9813 IST [Polaris SCA Package Manager Scan] INFO: Running command /Library/Java/JavaVirtualMachines/jdk-21.jdk/Contents/Home/bin/java -jar /Users/madhusud/.blackduck/bridge/tools/blackduck-detect/10.4.0/detect-10.4.0.jar --detect.cleanup=false --detect.bdio.file.name=scan --detect.bdio.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact --detect.output.path=/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect --detect.tools=DETECTOR --detect.component.location.analysis.enabled=true --blackduck.offline.mode=true --blackduck.offline.mode.force.bdio=true
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Self-Update feature is disabled because of the following reasons:
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Detect in offline mode is incompatible with the Self-Update feature.
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Detect-Self-Updater:  Black Duck URL is required for the Self-Update feature.
2025-11-13 11:34:50.7499 IST [Polaris SCA Package Manager Scan] INFO: ______     _            _
2025-11-13 11:34:50.7500 IST [Polaris SCA Package Manager Scan] INFO: |  _  \   | |          | |
2025-11-13 11:34:50.7500 IST [Polaris SCA Package Manager Scan] INFO: | | | |___| |_ ___  ___| |_
2025-11-13 11:34:50.7500 IST [Polaris SCA Package Manager Scan] INFO: | | | / _ \ __/ _ \/ __| __|
2025-11-13 11:34:50.7500 IST [Polaris SCA Package Manager Scan] INFO: | |/ /  __/ ||  __/ (__| |_
2025-11-13 11:34:50.7500 IST [Polaris SCA Package Manager Scan] INFO: |___/ \___|\__\___|\___|\__|
2025-11-13 11:34:50.7501 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:34:50.8767 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:34:50.8767 IST [Polaris SCA Package Manager Scan] INFO: Detect Version: 10.4.0
2025-11-13 11:34:50.8767 IST [Polaris SCA Package Manager Scan] INFO: 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Current property values:
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- --property = value [notes]
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode = true [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- blackduck.offline.mode.force.bdio = true [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.file.name = scan [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.bdio.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/bdio/blackduck_artifact [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.cleanup = false [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.component.location.analysis.enabled = true [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.excluded.directories = /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge [env] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.output.path = /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- detect.tools = DETECTOR [cmd] 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ------------------------------------------------------------
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect build date: 2025-04-24
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Source directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Output directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Run directory: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-04-50-835
2025-11-13 11:34:50.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] WARNING: --- Correlated Scanning is not available for Rapid/Stateless scan mode or offline scanning. A correlation ID will not be set.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Docker tool will not be run.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Bazel tool will not be run.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Will include the Detectors tool.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Searching for detectors.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Evaluating detectors. This may take a while.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detector Report
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======================================================================================================
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 	/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm (depth 0)
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 		NPM Package Lock: SUCCESS
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/package-lock.json
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 			Found file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/package.json
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detectors actions finished.
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project name: owasp-nodejs-goat
2025-11-13 11:34:51.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Project version: 1.3.0
2025-11-13 11:34:52.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:52.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Signature Scanner tool will not be run.
2025-11-13 11:34:52.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:52.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Vulnerability Impact Analysis tool will not be run.
2025-11-13 11:34:52.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:52.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- IaC Scanner tool will not be run.
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  Product Notice                                                                                #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  © 2024 Black Duck Software, Inc.                                                              #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  This Black Duck Component Locator and all associated documentation are proprietary            #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  to Black Duck Software, Inc. and may only be used pursuant to the terms and conditions of a   #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  written license agreement with Black Duck Software, Inc. All other use, reproduction,         #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  modification, or distribution of the Black Duck Component Locator or the associated           #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #  documentation is strictly prohibited.                                                         #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- #                                                                                                #
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ##################################################################################################
2025-11-13 11:34:53.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Running Component Locator v1.1.12 on /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis file saved at: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-04-50-835/scan/components-with-locations.json
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ----------------------------------
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Creating status file: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-04-50-835/status/status.json
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Skipping cleanup, it is disabled.
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Result ========
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Component Location Analysis File: /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/detect/runs/2025-11-13-06-04-50-835/scan/components-with-locations.json
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ======== Detect Status ========
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- NPM: SUCCESS
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Overall Status: SUCCESS - Detect exited successfully.
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- ===============================
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- 
2025-11-13 11:34:59.0000 IST [Polaris SCA Package Manager Scan][main] INFO: --- Detect duration: 00h 00m 09s 202ms
2025-11-13 11:34:59.4987 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'detect.completed'
2025-11-13 11:34:59.4989 IST [Polaris SCA Package Manager Scan] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.path'
2025-11-13 11:34:59.4991 IST [Polaris SCA Package Manager Scan] INFO: Adapter finished
2025-11-13 11:34:59.5437 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SAST(sastFull)" assessment with id "44ff459d-1628-4b4d-9931-ef8deef7dd54"
2025-11-13 11:34:59.5441 IST [Polaris Artifacts Uploader] INFO: uploading artifact for "SCA(scaPackage)" assessment with id "f3a92e15-3405-4f77-99b6-b061913dfe3e"
2025-11-13 11:35:00.9120 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip for "SCA(scaPackage)" assessment
2025-11-13 11:35:00.9591 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  14%  16384/114429
2025-11-13 11:35:00.9596 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  42%  49152/114429
2025-11-13 11:35:00.9665 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact:  71%  81920/114429
2025-11-13 11:35:00.9667 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SCA(scaPackage)" artifact: 100%  114429/114429
2025-11-13 11:35:00.9678 IST [Polaris Artifacts Uploader] INFO: Uploading artifact /Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip for "SAST(sastFull)" assessment
2025-11-13 11:35:01.0083 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:   4%  16384/386598
2025-11-13 11:35:01.0219 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  29%  114688/386598
2025-11-13 11:35:01.0428 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  55%  212992/386598
2025-11-13 11:35:01.0529 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact:  80%  311296/386598
2025-11-13 11:35:01.0541 IST [Polaris Artifacts Uploader] INFO: Uploading Progress of "SAST(sastFull)" artifact: 100%  386598/386598
2025-11-13 11:35:01.9686 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_sca_package_manager_scan/blackduck-sca-artifacts.zip"
2025-11-13 11:35:02.4603 IST [Polaris Artifacts Uploader] INFO: successfully uploaded artifact "/Users/madhusud/Jenkins_Testing/Nodes/workspace/thub_Polaris_Buildless_Scan_main@2/nodejs-npm/.bridge/polaris_coverity_capture/idir.zip"
2025-11-13 11:35:02.5192 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SCA(scaPackage)" assessment with id "f3a92e15-3405-4f77-99b6-b061913dfe3e"
2025-11-13 11:35:02.9480 IST [Polaris Artifacts Uploader] INFO: successfully resumed "SAST(sastFull)" assessment with id "44ff459d-1628-4b4d-9931-ef8deef7dd54"
2025-11-13 11:35:02.9698 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.artifacts.uploadSuccessful'
2025-11-13 11:35:02.9701 IST [Polaris Artifacts Uploader] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.artifacts.uploadSuccessful'
2025-11-13 11:35:02.9725 IST [Polaris Artifacts Uploader] INFO: Adapter finished
2025-11-13 11:35:03.0133 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SCA(scaPackage)" and id "f3a92e15-3405-4f77-99b6-b061913dfe3e"
2025-11-13 11:35:03.0137 IST [Polaris Waiter] INFO: Waiting for test with assessment type "SAST(sastFull)" and id "44ff459d-1628-4b4d-9931-ef8deef7dd54"
2025-11-13 11:35:03.3712 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "44ff459d-1628-4b4d-9931-ef8deef7dd54" is "Waiting for Capture"
2025-11-13 11:35:03.3786 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "f3a92e15-3405-4f77-99b6-b061913dfe3e" is "Queuing"
2025-11-13 11:35:13.8036 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SAST(sastFull)" and id "44ff459d-1628-4b4d-9931-ef8deef7dd54" is "Scanning"
2025-11-13 11:35:13.8038 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "f3a92e15-3405-4f77-99b6-b061913dfe3e" is "Scanning & Publishing"
2025-11-13 11:35:27.5549 IST [Polaris Waiter] INFO: Polling Test Manager: state of test with assessment type "SCA(scaPackage)" and id "f3a92e15-3405-4f77-99b6-b061913dfe3e" is "In Progress"
2025-11-13 11:35:37.8713 IST [Polaris Waiter] INFO: test with assessment type "SCA(scaPackage)" and id "f3a92e15-3405-4f77-99b6-b061913dfe3e" completed successfully
2025-11-13 11:35:37.8791 IST [Polaris Waiter] INFO: test with assessment type "SAST(sastFull)" and id "44ff459d-1628-4b4d-9931-ef8deef7dd54" completed successfully
2025-11-13 11:35:37.9003 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sast.tests.sastFull.completed'
2025-11-13 11:35:37.9008 IST [Polaris Waiter] INFO: Provided value for resource 'polaris.test.sca.tests.scaPackage.completed'
2025-11-13 11:35:37.9043 IST [Polaris Waiter] INFO: Adapter finished
2025-11-13 11:35:37.9734 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SAST(sastFull)" assessment...
2025-11-13 11:35:37.9739 IST [Polaris Policy Checker] INFO: Checking for policy violations for "SCA(scaPackage)" assessment...
2025-11-13 11:35:38.4023 IST [Polaris Policy Checker] INFO: no policies were violated to break the build
2025-11-13 11:35:38.4252 IST [Polaris Policy Checker] INFO: Adapter finished
2025-11-13 11:35:38.4712 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SAST(sastFull)" assessment
2025-11-13 11:35:38.4720 IST [Polaris Issues Fetcher] INFO: Fetching issues for "SCA(scaPackage)" assessment
2025-11-13 11:35:38.8457 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SAST(sastFull)" with id "44ff459d-1628-4b4d-9931-ef8deef7dd54"
 {
 "critical": 0,
 "high": 2,
 "informational": 0,
 "low": 25,
 "medium": 13
}
2025-11-13 11:35:38.8546 IST [Polaris Issues Fetcher] INFO: Successfully fetched issues for assessment type "SCA(scaPackage)" with id "f3a92e15-3405-4f77-99b6-b061913dfe3e"
 {
 "critical": 6,
 "high": 109,
 "informational": 0,
 "low": 15,
 "medium": 133
}
2025-11-13 11:35:38.8725 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.medium'
2025-11-13 11:35:38.8729 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.informational'
2025-11-13 11:35:38.8742 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.high'
2025-11-13 11:35:38.8746 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.low'
2025-11-13 11:35:38.8749 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.issues.critical'
2025-11-13 11:35:38.8752 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.informational'
2025-11-13 11:35:38.8757 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.high'
2025-11-13 11:35:38.8760 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.low'
2025-11-13 11:35:38.8763 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.medium'
2025-11-13 11:35:38.8767 IST [Polaris Issues Fetcher] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.issues.critical'
2025-11-13 11:35:38.8774 IST [Polaris Issues Fetcher] INFO: Adapter finished
2025-11-13 11:35:38.9362 IST [Polaris Status Provider] INFO: Results for test "SAST(sastFull)" with ID "44ff459d-1628-4b4d-9931-ef8deef7dd54" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/a200814e-6206-4a38-9f29-b68d067af36e/projects/953dcf56-3572-40ae-bc7c-8a17cc6ee4fd/tests/44ff459d-1628-4b4d-9931-ef8deef7dd54/detected-issues
2025-11-13 11:35:38.9369 IST [Polaris Status Provider] INFO: Results for test "SCA(scaPackage)" with ID "f3a92e15-3405-4f77-99b6-b061913dfe3e" are available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/a200814e-6206-4a38-9f29-b68d067af36e/projects/953dcf56-3572-40ae-bc7c-8a17cc6ee4fd/tests/f3a92e15-3405-4f77-99b6-b061913dfe3e/detected-issues
2025-11-13 11:35:38.9369 IST [Polaris Status Provider] INFO: Polaris issues view for project "buildless-scan", branch "main" is available at https://poc.polaris.blackduck.com/portfolio/portfolios/edf596d3-b54f-4a6b-9e5c-209f2e526c67/portfolio-items/a200814e-6206-4a38-9f29-b68d067af36e/projects/953dcf56-3572-40ae-bc7c-8a17cc6ee4fd/issues?branchId=90235b95-e899-45c7-a1d1-c11eeb0cf7ba
2025-11-13 11:35:38.9447 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SAST.tests.sastFull.summary.url'
2025-11-13 11:35:38.9451 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.test.SCA.tests.scaPackage.summary.url'
2025-11-13 11:35:38.9453 IST [Polaris Status Provider] INFO: Provided value for resource 'polaris.project.issues.url'
2025-11-13 11:35:38.9455 IST [Polaris Status Provider] INFO: Adapter finished
******************************* END EXECUTION OF BRIDGE CLI *******************************
[Security Scan] INFO: Retrieving the issue count from the scan results
[Security Scan] INFO: Total issues found: 303
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
Configuration: [githubOrg:polaris-jenkins-samples, repoName:buildless-scan, credentialsId:github-pat-logs-publisher, maxRetries:3, retentionCount:5, jobNamePrefixes:[MBP_Github_, MBP_, Github_, Pipeline_, Job_, Build_]]
[Pipeline] echo
Job Name: MBP_Github_Polaris_Buildless_Scan/main
[Pipeline] echo
Build Number: 2
[Pipeline] echo
GitHub Organization: polaris-jenkins-samples
[Pipeline] withCredentials
Masking supported pattern matches of $GITHUB_TOKEN
[Pipeline] {
[Pipeline] echo
Using configured repository name: buildless-scan
[Pipeline] echo
Target repository: polaris-jenkins-samples/buildless-scan
[Pipeline] echo
LogProcessor: captureJenkinsLogs called
```

---

*Log generated by Black Duck Logs Publisher*