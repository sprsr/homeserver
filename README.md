<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center">My Efficiency Focused Home Server</h3>

<div align="center">

  [![Status](https://img.shields.io/badge/status-active-success.svg)]() 
  [![GitHub Issues](https://img.shields.io/github/issues/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/issues)
  [![GitHub Pull Requests](https://img.shields.io/github/issues-pr/kylelobo/The-Documentation-Compendium.svg)](https://github.com/kylelobo/The-Documentation-Compendium/pulls)
  [![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> Documentation on my latest homeserver hardware and software stack. 
    <br> 
</p>

## 📝 Table of Contents
- [About](#about)
- [Hardware](#hardware)
- [Deployment](#deployment)
- [Usage](#usage)
- [Built Using](#built_using)
- [TODO](../TODO.md)
- [Contributing](../CONTRIBUTING.md)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

## 🧐 About <a name = "about"></a>
Write about 1-2 paragraphs describing the purpose of your project.

## 🏁 Hardware <a name = "hardware"></a>
List of Hardware: <br>
<p align="center">
<h3> Choosing A CPU: </h3> 
<h4> My Pick: Intel i3 9100T (40$ USD) </h4>
A good starting point is by evaluating other efficient systems.  It can be painful to find good power efficiency information online.  [This System Database](https://docs-google-com.translate.goog/?_x_tr_sl=nl&_x_tr_tl=en&_x_tr_hl=nl&_x_tr_pto=wapp&_x_tr_hist=true#gid=0) is the best resource I could find for comparing results of other systems.  You will notice that the majority of the most efficient systems recorded are a mix of Intel Core, Pentium, Celeron and Xeon Chips. <br>
Intel LGA 1151 Chips are a good balance of efficiency while performant.  Unless you plan to use a GPU in your system, make sure to avoid F Series Chips. 
The intention is to utilize Quick Sync Video for Media Streaming transcoding. Any Intel Series 7, 8, or 9 chip should be sufficiently powerful for most needs. <br><br>
- 7th Gen: VP9 8-Bit and 10-bit decoding, H.265/HEVC 8-bit and 10-bit decoding and encoding acceleration with 4:2:2 and 4:4:4 chroma subsampling, HDR10 Tone Mapping, and Open Source Media Shaders. <br><br>
- 8th Gen: VP9 12-bit & 12-bit 4:4:4 hardware decoding and HEVC 12-bit 4:2:0, 4:2:2 and 4:4:4 hardware decoding. Gen12 Xe will also support native AV1 decode, which includes 10-bit 4:2:0 16K stills and 10-bit 4:2:0 8K, 4K and 2K video. <br><br>
- 9th Gen: Intel Arc Alchemist (discrete GPUs) adds 8K 10-bit AV1 hardware encoding. <br><br>
I was able to find a secondhand T Series processor.  T Series is Intel's attempt at 'low-power desktop processors'.  However, these chips simply have a limited TDP.  This will rarely affect power consumption in our usecase, and likely never affect our idle consumption, however it can provide some peace of mind knowing your chips TDP when under load. I reccomend to use what ever Intel Gen 7-9 Chip you can find for a good price on Ebay. It is debatable whether Quad Core i3 chips have better idle consumption than other chips of the same generation, and even some of the most efficient machines recorded have been sporting i5 chips. 
</p>
<p align="center">
<h3> Choosing A CPU Cooler: </h3> 
<h4> My Pick: Supermicro SNK-P0046P (10.50$ USD) </h4>

</p>


### Prerequisites
What things you need to install the software and how to install them.

```
Give examples
```

### Installing
A step by step series of examples that tell you how to get a development env running.

Say what the step will be

```
Give the example
```

And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo.

## 🔧 Running the tests <a name = "tests"></a>
Explain how to run the automated tests for this system.

### Break down into end to end tests
Explain what these tests test and why

```
Give an example
```

### And coding style tests
Explain what these tests test and why

```
Give an example
```

## 🎈 Usage <a name="usage"></a>
Add notes about how to use the system.

## 🚀 Deployment <a name = "deployment"></a>
Add additional notes about how to deploy this on a live system.

## ⛏️ Built Using <a name = "built_using"></a>
- [MongoDB](https://www.mongodb.com/) - Database
- [Express](https://expressjs.com/) - Server Framework
- [VueJs](https://vuejs.org/) - Web Framework
- [NodeJs](https://nodejs.org/en/) - Server Environment

## ✍️ Authors <a name = "authors"></a>
- [@kylelobo](https://github.com/kylelobo) - Idea & Initial work

See also the list of [contributors](https://github.com/kylelobo/The-Documentation-Compendium/contributors) who participated in this project.

## 🎉 Acknowledgements <a name = "acknowledgement"></a>
- Hat tip to anyone whose code was used
- Inspiration
- References
