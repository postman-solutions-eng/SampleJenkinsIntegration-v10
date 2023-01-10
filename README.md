# SampleJenkinsIntegration-v10
In Postman v10, our generated sample code does not work to generate a working Jenkins integration in the Postman Jenkins Instance. The JSON here contains the correct pipeline configuration that should be used. Thanks to Carson Hunter for pointing us in the right direction. 



## Steps to Reproduce: 
1. Create an API within the API builder tab. 
2. Click “Test and Automate”. 
3. Select “Jenkins” under “Select your CI tool”. 
4. Complete steps to connect to Jenkins integration using credentials from Postman’s Jenkins implementation here. 
Click on “CI configuration”. 
5. Instructions allow you to select an OS and then generate command line configuration. “Copy this command and paste it to your build configuration file”
Upon copying into our Postman Jenkins implementation, this code will not work as curl is not installed by default. 
6. Instead we need to modify the code to mirror the following configuration due to our kubernetes configuration: https://jenkins.postmansolutions.com/job/ClaimsMobile2.0/configure

