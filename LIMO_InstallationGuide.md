# LIMO Installation Guide
## 1 IDE Setup
1. Install Eclipse (<https://www.eclipse.org/downloads/>). Any version should work
2. Install Google Web Toolkit
    1. Click Help – Install New Software
    2. In the ‘Work With’ textbox
        1. Paste: <http://storage.googleapis.com/gwt-eclipse-plugin/v3/release>
        2. 'Select All'
        3. Click 'Next' and 'Install'

## 2 Importing Source Code
1. Clone the repository via CLI
    1. SSH: git@github.com:purduedb/LIMO.git
    2. HTML: https://github.com/purduedb/LIMO.git
2. Import project in Eclipse -> location of cloned repo
3. Right click name of project –> properties –> project facets –> click on “Convert to faceted form” –> Set java version to 8 –> Apply –> OK
    1. If desired, most recent java version should work
4. Build path settings
    1. Right click name of project, select ‘build path’ –> ‘configure build path’
    2. In the Libraries tab, click Add Jars –> navigate to the project folder/war/WEB-INF/lib –> shift click and select all the jars in that folder –> Apply
    3. In the Source tab, Set default output folder to “\<name of project\>/war/WEB-INF/classes” –> Apply -> OK
    4. Right click name of project –> GWT –> Settings –> Check Use GWT –> Use default SDK –> OK

## 3 Running/Compiling Code
1. To run the code in local machine
    1. Right click name of project
    2. Click "Run as..." -> GWT Development Mode with Jetty –> Select GWTMaps.html –> OK
    3. You will see a URL for the web app on the right hand side, double click to open it on the browser
2. To compile source codes for deployment
    1. Right click name of project
    2. Select GWT – Compile
    3. Compiled files will be located under the war directory
    4. Push to repo