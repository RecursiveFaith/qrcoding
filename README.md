(this is still a draft research project)
 
# Agentic QR Codes

> ***What are the smallest arrangements of matter from which agentic processes can emerge?***

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

- Reimagines the browsers IndexedDB as a filesystem
  - IndexedDB stores values in `key : value` pairs
  - The `key` represents the filename and `value` represents the files contents
  - You can navigate these files by changing the `#hashstring` in the URL
- Add a `?prompt` to the URL to have an assistant edit the file
  - Depending on the API you are using you may need to add an API Key

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

