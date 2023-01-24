##Issue

1. Build the project or clean & build the project, GTMFetcherSession errors will appear

2. The errors are caused by changing the User Header Search Paths to: Pods/** (recursive)

3. To remove the errors, under User Header Search Paths, deleting Pods/**

4. User Header Search Paths > Pods/** (recursive) > is set for the bridging header

##This Xcode setting below was also changed but the main issue seems to be the Pods/** as described above


-Build Settings > Optimization Level, changed 'Release' from 'Fastest, Smallest' to 'None[-O0]', changed 'Optimization Level' from '<Multiple values>' to 'None[-O0]'
# GTMSessionFetcherIssue
