# TeamForge Customization Example

This project shows an example of how to customize the branding of TeamForge.

The customized CSS changes the navbar to blue using brute force. The more important aspect to this is the project structure itself and the building of the customization. Once you have that worked out, the details of the customized CSS is largely just a normal development and test effort.

## Building the Customization

The project uses Maven. To build the customization run this command from the project root:

    mvn package

The build process will produce a JAR file that contains the custom CSS file and a MANIFEST.MF that describes the customization and which is needed by TeamForge.

## Installing the Customization

The customization is installed via the TeamForge UI as a System Admin.  Go to the Admin menu and System Tools and then Customizations. Use the Create button to upload the JAR file that you built.

You may need to refresh or empty your cache for the new CSS file to load in your browser.

When I was testing my CSS changes, I would disable and delete the previous customization before uploading a new version.
