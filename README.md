# ChatBot Optimus
This project enables to run or deploy own ChatGPT-like coversational chatbot application.

### Description
OpenAI recently released the API to the most advanced language model GPT 3.5 turbo which powers ChatGPT and is 10 times cheaper than its predecessor GPT-3. 
Using that model and generating a OpenAI-Key for ownself this full-stack AI application is built which answers to queries just like ChatGPT. Users submit messages to a [SvelteKit](https://kit.svelte.dev) API Endpoint/Request Handler, which relays the messages to the ChatGPT API. The responses are then proxied back to the client via Server-Sent Evets (SSE) to stream the response in realtime.

### Tech-Stack Used
- Meta-Framework: [SvelteKit](https://kit.svelte.dev)
- Styles/Components: [TailwindCSS](https://tailwindcss.com) & [DaisyUI](https://daisyui.com)


## Steps to Run the Model Locally

Clone the Repository
```sh
git clone https://github.com/Siba-Prasad-Pattnaik/Optimus-AI-based-ChatBot)
```

Create a .env file within the same directory created and add your openAI key into it.
```sh
cd chatty && touch .env
echo OPENAI_KEY=<YOUR_API_KEY_HERE> >> .env
```
NOTE: You can get your open AI key from : https://platform.openai.com/account/api-keys

Install dependencies & start the dev server
```sh
pnpm i && pnpm run dev
```

You can now access the dev server running at [localhost:5173](https://localhost:5173)


