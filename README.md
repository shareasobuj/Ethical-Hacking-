# Ethical-Hacking-

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ethical Hacking Hub</title>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Fira Code', monospace;
      background-color: #0d0d0d;
      color: #e6e6e6;
      line-height: 1.6;
    }
    header {
      background: linear-gradient(90deg, #0f0f0f, #1a1a1a);
      padding: 20px;
      text-align: center;
      border-bottom: 2px solid #00ff99;
    }
    header h1 {
      color: #00ff99;
      font-size: 2.5rem;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #ccc;
      font-size: 1rem;
      transition: color 0.3s;
    }
    nav a:hover {
      color: #00ff99;
    }

    section {
      padding: 60px 20px;
      max-width: 900px;
      margin: auto;
      border-bottom: 1px solid #222;
    }
    section h2 {
      color: #00ff99;
      margin-bottom: 20px;
      font-size: 2rem;
    }
    section ul {
      padding-left: 20px;
    }
    section ul li {
      margin-bottom: 10px;
    }

    button {
      background-color: #00ff99;
      color: black;
      padding: 10px 20px;
      border: none;
      font-weight: bold;
      cursor: pointer;
      margin-top: 10px;
    }

    input, textarea {
      width: 100%;
      max-width: 500px;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #444;
      background-color: #1a1a1a;
      color: #fff;
    }

    footer {
      background-color: #111;
      text-align: center;
      padding: 20px;
      font-size: 0.9rem;
      color: #555;
    }

    #resourceList {
      margin-top: 10px;
      display: none;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 1.8rem;
      }
      nav a {
        display: block;
        margin: 10px 0;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>Ethical Hacking Hub</h1>
    <marquee> Developed By SOBUJ</marquee>
    <nav>
      <a href="#intro">Intro</a>
      <a href="#tools">Tools</a>
      <a href="#resources">Resources</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="intro">
    <h2>What is Ethical Hacking?</h2>
    <p>Ethical hacking is the practice of legally breaking into systems to discover potential vulnerabilities. It helps organizations strengthen their cybersecurity and prevent malicious attacks.</p>
  </section>

  <section id="tools">
    <h2>Popular Tools</h2>
    <ul>
      <li>Kali Linux - penetration testing OS</li>
      <li>Burp Suite - web vulnerability scanner</li>
      <li>Nmap - network mapper</li>
      <li>Wireshark - packet analyzer</li>
      <li>Metasploit - exploitation framework</li>
    </ul>
  </section>

  <section id="resources">
    <h2>Learning Resources</h2>
    <p>Click to view free ethical hacking resources:</p>
    <button onclick="toggleResources()">Show Resources</button>
    <div id="resourceList">
      <ul>
        <li><a href="https://www.hackthebox.com" target="_blank">Hack The Box</a></li>
        <li><a href="https://www.tryhackme.com" target="_blank">TryHackMe</a></li>
        <li><a href="https://owasp.org" target="_blank">OWASP</a></li>
        <li><a href="https://github.com/swisskyrepo/PayloadsAllTheThings" target="_blank">Payloads All The Things</a></li>
      </ul>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form onsubmit="handleSubmit(event)">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="4" placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
    <p id="formMsg"></p>
  </section>

  <footer>
    &copy; 2025 Ethical Hacking Hub | Designed with 💻 and ☕
  </footer>

  <script>
    function toggleResources() {
      const list = document.getElementById("resourceList");
      list.style.display = list.style.display === "none" ? "block" : "none";
    }

    function handleSubmit(e) {
      e.preventDefault();
      document.getElementById("formMsg").textContent = "Thanks! We'll get back to you soon.";
    }
  </script>
</body>
</html>
