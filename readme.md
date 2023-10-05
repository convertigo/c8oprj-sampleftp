


# sampleFTP

FTP sample project


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [CheckFile](#checkfile)
    - [List](#list)
    - [Upload](#upload)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     sampleFTP=https://github.com/convertigo/c8oprj-sampleftp.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     sampleFTP=https://github.com/convertigo/c8oprj-sampleftp/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __sampleFTP__ project


## Sequences

### CheckFile

<h1>This sequence is used to check one file name on a FTP server.</h1>

**outputs**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>file (0-1 time)</td><td>file name if found.</td>
</tr>
<tr>
<td>message (0-1 time)</td><td>Message if file not found.</td>
</tr>
<tr>
<td>hasFile</td><td>true/false</td>
</tr>
<tr>
<td>success</td><td>true/false</td>
</tr>
<tr>
<td>error (0-1 time)</td><td>Error message if any.</td>
</tr>
</table>

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>file</td><td>FTP file name to search for</td>
</tr>
<tr>
<td>host</td><td>FTP server host name or IP</td>
</tr>
<tr>
<td>password</td><td>FTP password</td>
</tr>
<tr>
<td>port</td><td>FTP port number</td>
</tr>
<tr>
<td>source</td><td>FTP source folder</td>
</tr>
<tr>
<td>username</td><td>FTP user name</td>
</tr>
</table>

### List

<h1>This sequence is used to obtain a list of file names in a directory (source) or current working directory (source is null).</h1>

**outputs**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>files with length, array of file (0-n times)</td><td>file names found in FTP server directory.</td>
</tr>
<tr>
<td>success</td><td>true/false</td>
</tr>
<tr>
<td>error (0-1 time)</td><td>Error message if any.</td>
</tr>
</table>

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>host</td><td>FTP server host name or IP</td>
</tr>
<tr>
<td>password</td><td>FTP password</td>
</tr>
<tr>
<td>port</td><td>FTP port number</td>
</tr>
<tr>
<td>source</td><td>FTP source folder</td>
</tr>
<tr>
<td>username</td><td>FTP user name</td>
</tr>
</table>

### Upload

<h1>This sequence is used to upload one file on a FTP server.</h1>

**outputs**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>success</td><td>true/false</td>
</tr>
<tr>
<td>error (optional)</td><td>Error message.</td>
</tr>
</table>

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>destination</td><td>FTP destination folder</td>
</tr>
<tr>
<td>file</td><td>source file path</td>
</tr>
<tr>
<td>host</td><td>FTP server host name or IP</td>
</tr>
<tr>
<td>password</td><td>FTP password</td>
</tr>
<tr>
<td>port</td><td>FTP port number</td>
</tr>
<tr>
<td>username</td><td>FTP user name</td>
</tr>
</table>



