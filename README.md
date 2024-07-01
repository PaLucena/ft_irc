
<h1 align="center">ft_irc</h1>
  
<h2>Description</h2>
  <p><strong>ft_irc</strong> is a project from the 42 cursus that involves implementing an IRC (Internet Relay Chat) server from scratch, following the specifications of the RFC 2812 protocol. The main objective is to understand the internal workings of network communication protocols and acquire skills in systems programming, socket handling, and concurrency management.</p>
  <div align="center"><img alt="Diagram" src="https://github.com/PaLucena/ft_irc/blob/master/img/architecture.png"></div>

<h2>Table of Contents</h2>
  <ul>
      <li><a href="#requirements">Requirements</a></li>
      <li><a href="#installation">Installation</a></li>
      <li><a href="#usage">Usage</a></li>
      <li><a href="#supported-commands">Supported Commands</a></li>
      <li><a href="#project-structure">Project Structure</a></li>
      <li><a href="#authors">Authors</a></li>
      <li><a href="#license">License</a></li>
  </ul>

<h2>Requirements</h2>
  <p>To compile and run the project, you will need:</p>
  <ul>
      <li>A Unix operating system (Linux or macOS).</li>
      <li>A C++ compiler (compatible with C++98).</li>
      <li>Make.</li>
  </ul>

<h2>Installation</h2>
  <p>Clone the project repository and navigate to the main directory:</p>
  <pre><code>
    git clone https://github.com/PaLucena/ft_irc.git && cd ft_irc
  </code></pre>
  <p>Compile the project using the included Makefile:</p>
  <pre><code>make</code></pre>
  <p>This will generate the <code>ircserv</code> executable in the current directory.</p>

<h2>Usage</h2>
  <p>To start the IRC server, run the following command:</p>
  <pre><code>./ircserv &lt;port&gt; &lt;password&gt;</code></pre>
  <ul>
      <li><code>&lt;port&gt;</code>: The port on which the server will listen (e.g., 6667).</li>
      <li><code>&lt;password&gt;</code>: The password required to connect to the server.</li>
  </ul>
  <p>Example:</p>
  <pre><code>./ircserv 6667 mypassword</code></pre>

<h2>Supported Commands</h2>
  <p>The IRC server supports a series of standard commands defined in RFC 2812. Some of the implemented commands include:</p>
  <ul>
      <li><code>PASS</code>: Password to access server.</li>
      <li><code>NICK</code>: Change username.</li>
      <li><code>USER</code>: Register username.</li>
      <li><code>JOIN</code>: Join a channel.</li>
      <li><code>PRIVMSG</code>: Send a private message to a user or channel.</li>
      <li><code>MODE</code>: Change a channel's mode.</li>
      <li><code>PART</code>: Leave a channel.</li>
      <li><code>INVITE</code>: Invite user to a channel.</li>
      <li><code>KICK</code>: Eject a client from the channel.</li>
      <li><code>TOPIC</code>: Change or view the channel's topic.</li>
  </ul>
  <p>For a complete list of commands and their functionality, refer to <a href="https://tools.ietf.org/html/rfc2812" target="_blank">RFC 2812</a>.</p>

<h2>Project Structure</h2>
  <p>The project is organized into the following files and directories:</p>
  <ul>
      <li><code>src/</code>: Contains the source code of the IRC server.</li>
      <li><code>include/</code>: Contains the header files.</li>
      <li><code>Makefile</code>: Build script to generate the executable.</li>
      <li><code>README.md</code>: Project documentation.</li>
  </ul>

<h2>Authors</h2>
  <p>This project was developed by the 42 cursus students:</p>
  <ul>
      <li><a href="https://github.com/ealgar-c" target="_blank">Enrique Algar Ceular</a></li>
      <li><a href="https://github.com/PaLucena" target="_blank">Pablo Lucena González</a></li>
  </ul>

<h2>License</h2>
  <p>This project is licensed under the MIT License. See the <code>LICENSE</code> file for more details.</p>
