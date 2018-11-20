# Links

# https://github.com/google/clasp#login
# https://github.com/gsuitedevs/gmail-add-ons-samples/tree/master/github
# https://developers.google.com/apps-script/reference/card-service/card
# https://itnext.io/google-apps-script-creating-stateful-gmail-add-ons-part-one-89186ae17f7e
# https://github.com/ezrasandzerbell/Gmail-addon-stateful-demo


Deploy the add-on

Deploy the add-on by following these steps:

    Create a new project:

    clasp create "Git Info"

    Push the code:

    clasp push

    Tag a version:

    clasp version 'Push from github'

    Deploy the add-on:

    clasp deploy 1 'test'

    Verify the deployments:

    clasp deployments

Note the deployment ids. There will be two deployments, one for the tagged version, another for the @HEAD version. Use the @HEAD deployment when installing the add on if you intend to modify or experiment with the code.


# About the “Volunteer Registration” Demo App

## Article Tutorial: https://medium.com/@ezra_69528/google-apps-script-creating-stateful-gmail-add-ons-part-one-89186ae17f7e

## Application Summary: In this demo, the user has signed up for a trade show and will be volunteering for a day or night shift on behalf of their company.

## Application Features: This app showcases several Gmail Add-Ons features, including multi-card navigation, form input retrieval with persistent state (user props storage), and a “confirm” button that prints user data as a canned email response.

## Application UI: The application consists of two cards (shown below) with a Universal Settings icon (triple dot) in the header for navigation.

## Application UX: selects a company that they work for, which causes an employee list to appear in the dropdown menu. These settings are saved and the user navigates to a new card where they can choose to volunteer for a day or night shift. When finished, they confirm and the Add-On will create an email reply with canned response.
