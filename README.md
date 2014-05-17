social-notif-fake-smtp
======================

Makes the fake smtp mail service what uses for exo social notification sending mail.

1. Checkout the repository: git clone git@github.com:Nilhcem/FakeSMTP.git and compile by maven
2. Checkout the repository: git clone git@github.com:exosocial/social-notif-fake-smtp.git
3. Package by maven: mvn clean install
4. Copy jar to extensions/fake-smtp/lib then, copy war to extensions/fake-smtp/webapps
5. Goto extension folder, copy fake-smtp to PLATFORM_TOMCAT/extensions folder
6. Run the following command to install the fake-smtp project.

    Linux/Mac: ./extension.sh --install custom-extension

    Windows: extension.bat --install custom-extension

7. Start FakeSMTP mail server. 

java -jar fakeSMTP.jar -o OUTPUT_FOLDER_MAIL

8. Start server with port 2525

9. Run eXo PLF tomcat bundle.