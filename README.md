<h1>QR</h1>
<blockquote>A recursive, generative QR Code framework</blockquote>

<br>
<hr>
<br>

<h1>Getting started</h1>

<h2>(option 1) Clone or download the source code locally</h2>
<blockquote>[coming soon]</blockquote>

<br>
<hr>
<br>

<h1>(Optional) Extract source code from QR Code</h2>
<p>The source code is small enough to be embedded completely inside a standard QR Code, so if your device isn't connected to the network the default camera app (likely) automatically reads QR Codes. If not, any QR Code app or QR Code Scanner can read these since they use standard encoding
<p>"Standard QR Codes" range from version 1 to 40, or about 17 bytes to 2953 bytes of data. Those numbers are for raw byte data though, QR Codes can encode different types of data. For numeric characters the range is more like 41 - 7089 numeric characters or 25 - 4296 for alphanumerics</p>
<p>This is still very experimental and designed for easily loading onto retro and embedded devices that aren't connected, as well as for creative archiving and distribution. If you scan one of the codes below you'll get the contents of index.html, and can run this project on that device without a traditional network connection</p>


<table>
  <thead>
    <tr>
      <th colspan=2>index.html</th>
    </tr>
    <tr>
      <th>Compressed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <div>QR Code version = 40</div>
        <div>character count = 2837</div>
        <div>data bits = 22716</div>
      </td>
    </tr>
    <tr>
      <td>
        <img title="qr.0.0.1" src="https://github.com/user-attachments/assets/edd2386e-0b24-4ba7-9aee-d5ca61f42553">
      </td>
    </tr>    
  </tbody>
</table>

<h3>Maximum Standard Limits</h3>
<p>Subtract the above values from the below limits to estimate how much more custom data you can squeeze into a QR code. This gives you considerable</p>
<div>QR Code version = 40 (177x177)</div>
<div>character count = 7089</div>
<div>data bits = 23624 (~3KB)</div>

<h3>Generating QR Codes</h3>
For now I'm making them here: https://www.nayuki.io/page/qr-code-generator-library
