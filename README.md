# joshfarias.github.io

## Programming Projects

<h2>
  <img src="https://github.com/joshfarias/Python/raw/main/images/python-logo.png" height="100">
</h2>

<h3>Chatbot using text-davinci-003 Model from OpenAI</h3>
<p><a href="https://github.com/joshfarias/Python/blob/main/src/davinci-003-chatbot.py"><strong>davinci-003-chatbot.py</strong></a></p>
<p>This program uses <a href="https://openai.com/blog/openai-api">OpenAI's API</a> to generate responses to user prompts and questions in an interactive chatbot format. The responses generated are based on OpenAI's text-davinci-003 language model. To end the chat the user can enter the keyword <code>end</code>.</p>
<p>Below is an screenshot containing a brief conversation with the chatbot:</p>

<h2>
<img src="https://github.com/joshfarias/Python/blob/main/images/davinci-003-chatbot.png" alt="python logo" height="400">
</h2>

<h4>Notes</h4>
<ul>
<li>Users must have the OpenAI API library for Python installed in order for this program to work. The library can be installed using the following pip command: <code>pip install openai</code></li>
<li>The program has the API key set as an environment variable by default, the code can however be modified in the following ways so that the user can set up their API key differently:
  <ul>
  <li>Use a configuration file to store the API key</li>
  <li>Pass the API key through a command-line argument</li>
  <li>Use a keyring library</li>
  <li>Hardcode the API key (not recommended)</li>
  </ul>
</li>
<li>The <code>openai.Completion.create()</code> function call includes several parameters that can be adjusted to change the behavior of the chatbot. More information regarding the parameters can be found on <a href="https://platform.openai.com/docs/api-reference/completions/create">OpenAI's API documentation</a>.</li>
</ul>

<h3>AI Image Generator using OpenAI's DALL-E Model</h3>
<p><a href="https://github.com/joshfarias/Python/blob/main/src/DALLEImageGenerator.py">DALLEImageGenerator.py</a></p>
<p>This program uses <a href="https://openai.com/blog/openai-api">OpenAI's API</a> to generate images based on user prompts using OpenAI's DALL-E model. For best results, user prompts should be clear and concise. For example <code>cat</code> vs <code>orange cat sitting on a windowsill overlooking a city skyline at sunset, photorealistic</code>:</p>

<p><img src="https://github.com/joshfarias/Python/blob/main/images/cat.png" alt="Orange Cat"> <img src="https://github.com/joshfarias/Python/blob/main/images/better-cat-prompt.png" alt="Orange Cat Sitting on Windowsill"></p>

<h4>Notes</h4>
<ul>
<li>Users must have the OpenAI API library for Python installed in order for this program to work. The library can be installed using the following pip command: <code>pip install openai</code></li>
<li>The program has the API key set as an environment variable by default, the code can however be modified in the following ways so that the user can set up their API key differently:
  <ul>
    <li>Use a configuration file to store the API key</li>
    <li>Pass the API key through a command-line argument</li>
    <li>Use a keyring library</li>
    <li>Hardcode the API key (not recommended)</li>
  </ul>
</li>
<li>By default the program is set to generate a single image with a resolution of <code>256x256</code>. This was done for prompt testing purposes due to the greater charges OpenAI places on higher resolution images. This however can easily be changed by modifying the <code>size</code> parameter in the <code>openai.Image.create()</code> function call to a greater resolution such as <code>1024x1024</code> and by modifying the <code>n</code> parameter to a set number of how many images you want such as <code>3</code>.</li>
</ul>
