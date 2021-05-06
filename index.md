## C# configuration with Visual Studio Code running on CentOS 7
### To install Visual Studio Code in CentOS 7, follow this link
<a>https://mbmasadeh.github.io/VisualStudioCodeSetupCentOS/</a>

### Open VS code from the termnal by typing this command
<pre><code>$ code </code></pre>

<p>Then inside it open a new terminal from the menu above - Run </p>
<p>We need to install all the required SDK packeges to run C# smoothly</p>

Add the Microsoft package signing key to your list of trusted keys and add the Microsoft package repository
<pre><code>$ sudo rpm -Uvh https://packages.microsoft.com/config/centos/7/packages-microsoft-prod.rpm</code></pre>

### Install the SDK
<pre><code>$ sudo yum install dotnet-sdk-5.0 </code></pre>

### Install the runtime
<pre><code>$ sudo yum install aspnetcore-runtime-5.0</code></pre>

### Test your work
<p>Instaltion and confiuration is done, to test your work type this command</p>
<pre><code>$ dotnet </code></pre>

<p>The result is:</p>
<pre><code>
Usage: dotnet [options]
Usage: dotnet [path-to-application]

Options:
  -h|--help         Display help.
  --info            Display .NET information.
  --list-sdks       Display the installed SDKs.
  --list-runtimes   Display the installed runtimes.

path-to-application:
  The path to an application .dll file to execute.
  </code></pre>

### Create your first application
<p>To make the first .Net application, type this command which will start a new console application</p>
<pre><code>$ dotnet new consol -o MyFirstApplication </code></pre>
<p>Note that this is a Concol application</p>

<pre><code>$ dotnet new api -o ApiApplication </code></pre>
<p>Note that this is an Api application</p>
<p>To run you application, type this command <p>
<p>First go inside "YourApplicationName" project</p>
<pre><code>$ cd YourApplicationName </code></pre>

<p>Then run it</p>
<pre><code>$ dotnet run </code></pre>

<p>The result is hallow word</p>

<p>Thats all....!</p>
