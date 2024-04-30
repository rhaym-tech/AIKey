<h1 align="center">
  <br>
  <a href="https://github.com/rhaym-tech"><img src="https://user-images.githubusercontent.com/43763935/220091266-4ee56084-67c6-439b-818d-886acaaad847.png" height="200" alt="OpenAI authenticator"></a>
  <br>
  AIKey
  <br>
</h1>

<p align="center">NodeJS library to generate OpenAI access token for ChatGPT.</p>

<p align="center">Made by <a href="https://github.com/rhaym-tech">rhaym-tech</a>

<br>

<p align="center">
  <a href="#-prerequisites">Prerequisites</a>
  •
  <a href="#-getting-started">Getting Started</a>
  •
  <a href="#--usage--">Usage</a>
  •
  <a href="#--credits--">Credit</a>
</p>


## [Download](https://github.com/rhaym-tech/AIKey/releases/download/1.0.2/Aikey.zip)


### **Print the Access Token**
```js
import OpenAITokenGen from "aikey";

  const generator = new OpenAITokenGen();

  const Access_Token = await generator.login("OpenAI email", "OpenAI password")
  console.log(Access_Token);
```
### Use it with ChatGPT ( ChatGPTUnofficialProxyAPI )

```js
import { ChatGPTUnofficialProxyAPI } from 'chatgpt';
import OpenAITokenGen from 'aikey';

async function ChatGPT() {
  const generator = new OpenAITokenGen();
  const api = new ChatGPTUnofficialProxyAPI({
    accessToken: await generator.login("OpenAI email", "OpenAI password");
  })

  const response = await api.sendMessage('Hello World!')
  console.log(response.text)
}
```


<br>
<h1 align="center"> 🤝 Credits 🤝 </h1>
<a herf="https://github.com/rhaym-tech">@rhaym-tech</a>: Project owner
<br>
<a herf="https://github.com/transitive-bullshit">@transitive-bullshit</a>: Node.js client for ChatGPT developer
<br>
<a herf="https://github.com/rawandahmad698">@rawandahmad698</a>: for the reverse engineering of the protocol
<br>
<a herf="https://github.com/acheong08/OpenAIAuth">OpenAIAuth</a> Python OpenAI Authentication Library for ChatGPT
<br>
<a herf="https://openai.com">OpenAI</a>: OpenAI API owner
