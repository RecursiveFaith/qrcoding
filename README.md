(this is still a draft research project)
 
# Agentic QR Codes

> ***Research Questions:*** _Is it possible to create a single self-contained QR code that generates a Large Language Model simulated Operating System? Can an LLM OS be used to generate full-dive mixed realities?_

## Technical Foundation

Standard QR codes offer remarkable data capacity, with Version 40 (177x177) supporting up to 2,953 bytes of raw data with error correction. They are robust and can be encoded into various mediums and scanned from nearly any device

<table>
  <thead>
    <tr>
      <th colspan=2>
        QR codes are medium agnostic
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <a href="https://www.youtube.com/watch?v=w5ebcowAJD8">
          <img title="Veritassium: I built a QR code with my bare hands to see how it works" src="https://img.youtube.com/vi/w5ebcowAJD8/0.jpg" width=354>
        </a>
      </td>
      <td>
        <a href="https://www.righto.com/2009/01/qr-codes-in-lego.html">
          <img title="Ken Shirriff: QR codes in Lego" src="https://static.righto.com/images/legoqr.jpg" width=354>
        </a>
      </td>
    </tr>    
  </tbody>
</table>

Agentic QR codes are ones that contain all the code necessary to bootstrap an LLM OS. An LLM OS is an Operating System metaphor that imagines AI as the Central Processing Units of virtual machines

<a href="https://huggingface.co/blog/shivance/illustrated-llm-os"><img width="1440" title="Illustrated LLM OS: An Implementational Perspective" src="https://github.com/user-attachments/assets/7c3d07f4-a3f7-4296-9235-d640bba1fce2" /></a>

## Browser Implementations

The following QR codes all encode the same minimal serverless LLM OS as a static HTML, they just differ in their LLM API implementation. Scan the code to copy + paste the string into a `.html` file, then open that file in the browser. Alternatively, you can view the source code in this repo and generate your own codes.

### How it works
> **Note:** I'm still editing this section

- Reimagines IndexedDB as the filesystem
  - There is a table called `page`
  - The `window.location` `#hashstring` is used as the key
  - The value is rendered by the browser as raw HTML + JavaScript
- By default each `#hashstring` is displayed in a textarea annd iframe
  - The textarea lets you edit the `page` contents
  - The iframe renders it, applying `<style>` and running `<script>` tags
- The URL itself is also a prompting interface
  - Add a `?prompt` to the URL to have an LLM edit the page
  - If you are using a cloud hosted LLM like ChatGPT it'll ask for an API key
  - The prompt gets sent with `<url>window.location</url><page>contents of #hastring</page>` and a system prompt
- Opening two tabs to the same `#hashstring` will keep them synced as you edit
  - This prevents accidental edits
  - Lets you view and edit different parts of the same page
  - Uses the browsers' Broadcasting and Observable APIs

<table>
  <thead>
    <tr>
      <th colspan=2><h3>OpenRouter</h3></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <ul>
          <li>Free API keys available https://openrouter.ai</li>
        </ul>
        <img src="./openrouter.0.1.png" width=354>
      </td>
      <td>
      </td> 
    </tr>    
  </tbody>
</table>

## Development Tools

QR code generation is currently handled through the [Nayuki QR Code Generator Library](https://www.nayuki.io/page/qr-code-generator-library), which provides robust encoding capabilities for various data formats.

## Future Development

The project is evolving to include:
- An advanced editor interface
- Local development options
- Enhanced code generation capabilities

This experimental platform opens new possibilities for creative archiving and distribution, particularly focused on retro and embedded devices operating in offline environments.

## Core Capabilities

The source code is designed to be entirely self-contained within a standard QR code. Most modern devices can read these codes through their default camera app, while any QR code scanner app serves as a fallback option.

**Data Encoding Ranges:**
- Raw byte data: 17 to 2,953 bytes
- Numeric characters: 41 to 7,089 characters
- Alphanumeric: 25 to 4,296 characters

