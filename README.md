
<body>
    <h1>Claude Code Setup with OpenRouter</h1>
    
  <p>Quick guide to configure Claude Code with OpenRouter for using various AI models.</p>

  <h2>1. Install Claude Code</h2>
  
  <p><b>Download via npm:</b></p>
  <pre><code>npm install -g @anthropic-ai/claude-code</code></pre>
  
  <p><b>Note:</b> Requires Node.js 18+ installed on your system.</p>

  <h2>2. Create Configuration Directory</h2>
  
  <p>Navigate to your home directory and create the <code>.claude</code> folder:</p>
  
  <pre><code>cd ~
mkdir .claude
cd .claude</code></pre>

  <h2>3. Create settings.local.json File</h2>
  
  <p>Inside the <code>.claude</code> directory, create a file named <code>settings.local.json</code> with this content:</p>
  
  <pre><code>{
  "env": {
    "ANTHROPIC_BASE_URL": "https://openrouter.ai/api",
    "ANTHROPIC_AUTH_TOKEN": "your_openrouter_api_key",
    "ANTHROPIC_API_KEY": "",
    "ANTHROPIC_MODEL": "openrouter/free" //Replace with your open router model name
  }
}</code></pre>

  <h2>4. Configure Your Settings</h2>
  
  <p>Replace the following values:</p>
  
  <ul>
      <li><b>ANTHROPIC_AUTH_TOKEN:</b> Your OpenRouter API key from <a href="https://openrouter.ai/">openrouter.ai</a></li>
      <li><b>ANTHROPIC_MODEL:</b> Your desired model (see examples below)</li>
  </ul>
  
  <p><b>Popular Models:</b></p>
  <ul>
      <li><code>anthropic/claude-3.5-sonnet</code></li>
      <li><code>anthropic/claude-3-opus</code></li>
      <li><code>openai/gpt-4-turbo</code></li>
      <li><code>google/gemini-pro</code></li>
  </ul>

  <h2>5. Run Claude Code</h2>
  
  <p>Start Claude Code with:</p>
  <pre><code>claude</code></pre>
  
  <p>Claude Code will now use OpenRouter as the backend.</p>

  <h2>Troubleshooting</h2>
  
  <p><b>Command not found:</b> Add npm's global bin directory to your PATH.</p>
  <p><b>Invalid API key:</b> Verify your OpenRouter API key at <a href="https://openrouter.ai/keys">openrouter.ai/keys</a></p>
  
  <hr>
  
  <p><b>Resources:</b></p>
  <ul>
      <li><a href="https://docs.anthropic.com/claude-code">Claude Code Documentation</a></li>
      <li><a href="https://openrouter.ai/docs">OpenRouter Documentation</a></li>
      <li><a href="https://openrouter.ai/models">Available Models</a></li>
  </ul>

</body>
