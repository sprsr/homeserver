<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center"> Complete Home Server Ecosystem </h3>

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
- [Server Hardware](#server_hardware)
- [Server OS](#server_os)
- [Server Services](#server_services)
- [Clients](#clients)
- [Automation](#automation)
- [Privacy](#privacy)
- [Authors](#authors)
- [Acknowledgments](#acknowledgement)

## 🧐 About <a name = "about"></a>
Write about 1-2 paragraphs describing the purpose of your project.

## 🏁 Hardware <a name = "hardware"></a>
  
List of Hardware: <br>
<p align="center">
<h3> Choosing A CPU: </h3> 
<h4> My Pick: Intel i3 7100 (10$ USD) </h4>
A good starting point is by evaluating other efficient systems.  It can be painful to find good power efficiency information online.  [This System Database](https://docs-google-com.translate.goog/?_x_tr_sl=nl&_x_tr_tl=en&_x_tr_hl=nl&_x_tr_pto=wapp&_x_tr_hist=true#gid=0) is the best resource I could find for comparing results of other systems.  You will notice that the majority of the most efficient systems recorded are a mix of Intel Core, Pentium, Celeron and Xeon Chips. <br>
Intel LGA 1151 Chips are a good balance of efficiency while performant.  Unless you plan to use a GPU in your system, make sure to avoid F Series Chips. 
The intention is to utilize Quick Sync Video for Media Streaming transcoding. Any Intel Series 7, 8, or 9 chip should be sufficiently powerful for most needs. <br><br>
- 7th Gen: VP9 8-Bit and 10-bit decoding, H.265/HEVC 8-bit and 10-bit decoding and encoding acceleration with 4:2:2 and 4:4:4 chroma subsampling, HDR10 Tone Mapping, and Open Source Media Shaders. <br><br>
- 8th Gen: VP9 12-bit & 12-bit 4:4:4 hardware decoding and HEVC 12-bit 4:2:0, 4:2:2 and 4:4:4 hardware decoding. Gen12 Xe will also support native AV1 decode, which includes 10-bit 4:2:0 16K stills and 10-bit 4:2:0 8K, 4K and 2K video. <br><br>
- 9th Gen: Intel Arc Alchemist (discrete GPUs) adds 8K 10-bit AV1 hardware encoding. <br><br>
I was able to find a secondhand T Series processor.  T Series is Intel's attempt at 'low-power desktop processors'.  However, these chips simply have a limited TDP.  This will rarely affect power consumption in our usecase, and likely never affect our idle consumption, however the price was right, and I suppose gives some peace of mind knowing your chips TDP when under load. I reccomend to use what ever Intel Gen 7-9 Chip you can find for a good price on Ebay. It is debatable whether Quad Core i3 chips have better idle consumption than other chips of the same generation, and even some of the most efficient machines recorded have been sporting i5 chips. 
</p>


<h3> CPU Recomendations: </h3> 
If you want 

<h3> Choosing A CPU Cooler: </h3> 
<h4> My Pick: Supermicro SNK-P0046P (10.50$ USD) </h4>
This passive cooler should be sufficient for a low tdp quad core, however I am not 100% sure I will not need an active cooler.  Will update depending on my temps. 

<h3> Choosing A Motherboard: </h3> 
<h4> My Pick: Supermicro X11SSH-F (90$ USD) </h4>
Generally, Mini ITX Motherboards have far better consumption than any ATX variant.  In the perfect world, I would suggest always going with a non gaming mini ITX, however, due to the market for home server builds, it can be very difficult to find boards with 
sufficient IO for a decent price. I searched for a C246 chipset mini ITX for weeks, and could find nothing under $100.  Eventually I stumbled across this micro ATX C246 Chipset board on ebay.  The X11SSH-F supports 8sata ports, and a single M.2 M Key slot.  <br><br>
If budget is non existant to you, the ideal motherboard would probably be a Fujitsu D36XXB series board that supports ECC.  These boards can have <5W idle consumption while supporting 6 sata ports.  However, due to enthusiasts you will struggle to find one of these boards alltogether, and will likely pay north of $300 for a 5+ year old cheap motherboard.  Avoid any gaming motherboards, as they typically have cutting edge features that consume more power. 

<h3> Choosing Memory: </h3> 
<h4> My Pick: A-Tech 32 GB DDR4 2400 MHz ECC DIMM RAM  (40$ USD) </h4>
Ram does not play much of a role in Power Consumption thankfully, so feel free to choose whatever you can find for cheapest. My Motherboard supports 64 GB ECC DDR4 DIMM Ram, so I chose two sticks for 32GB to allow potential future upgrades.  The services I will run 24/7 will consume less than 8GB at max load, leaving plenty of free ram for future additions and workstation use. If you plan on sticking with the spirit of my build, focused in efficiency, it is best to avoid any RGB gaming ram to save a watt or two.

<h3> Choosing a Power Supply: </h3> 
<h4> My Pick: 550W EVGA Supernova G2 (40$ USD) </h4>
For absolute best efficiency, it is best to use a PicoPSU.  I reccomend sticking with the three official models of PicoPSU (80W, 90W, 160W). My ARM server cluster ran on a 160W PicoPSU with 4 M.2 Drives and Three Sata Drives with no issues.  Using a Standard ATX Power Supply, we will see less efficiency at idle.  Even Gold rated 80+ efficiency ATX PSUs such as my selection are usually only at 70% efficiency in the best case scenario at 10% load.  The 80+ efficiency rating is only relevant above 20% load.  My choice to chose an ATX is because of my large case selection, future proofing for a large amount of disc drives, and somewhat experimental.  I may swap the ATX out with a PSU if my results are less than desireable. 

<h3> Choosing a Case: </h3> 
<h4> My Pick: Fractal Node 804  (100$ USD) </h4>
Find whatever case fits your budget and needs, as there is no need to worry about power consumption (obviously)  After running barebaones with no case for over a year on my home server cluster, I decided on the Fracal Node 804.  This is an old cube case with support for 10 3.5 drives and 2 2.5 drives. 
This case is quite expensive when compared to ebay finds, but planning to run my system with a passive cpu cooler so I want to ensure good airflow with excellent drive support. 

<h3> Choosing Drives: </h3> 
<h4> My Pick: 1TB Western Digital SN730 (~$47)  Single Seagate 10TB 3.5  (~$70 USD) </h4>
Too many home server builders load their system up with drives as soon as they build (Even some efficiency enthusiasts!).  I don't understand this, as you are simply wasting money and power.  I reccomend starting with a 1 TB NVME for your OS and File System for programs, followed by 2.5/3.5 Sata Drives that support your current needs. <br> <br>

The hardware I chose was based on what I could find for a good used price, not neccesarily what I would build if I was purchasing new parts.  
Below shows the cost and value of my build.  Note that I am migrating storage from my previous Home server, negating the paid price for drives.

| Component                    | Paid Price | Market Value |
| ---------------------------- | ---------- | ------------ |
| i3 7100                      |        $10 | $20          |
| SuperMicro C246 Micro ATX    |        $90 | ~$180        |
| 32GB DDR4 ECC DIMM RAM       |        $40 | $40          |
| 550 Watt PSU                 |        $40 | $80          |
| Fractal Node 804             |       $100 | $140         |
| 1TB WD SN730                 |          ~ | $70          |
| 10TB Seagate 3.5 Drive       |          ~ | $180         |
| Total:                       |       $244 | $750         |  
  <br>
<h3> Other Recommendations: </h3> 
Intel N100 Motherboard <br>
Intel N5105 Motherboard <br>
Any N100/N5105 Nuc or Mini PC with sufficent expandable storage <br>
</p>
## Server Operating System <a name = "server_os"></a>

Operating System Arch Linux





## ⛏️ Built Using <a name = "built_using"></a>
- [MongoDB](https://www.mongodb.com/) - Database
- [Express](https://expressjs.com/) - Server Framework
- [VueJs](https://vuejs.org/) - Web Framework
- [NodeJs](https://nodejs.org/en/) - Server Environment

## ✍️ Authors <a name = "authors"></a>
- [@sprsr](https://github.com/sprsr)

See also the list of [contributors](https://github.com/kylelobo/The-Documentation-Compendium/contributors) who participated in this project.

## 🎉 Acknowledgements <a name = "acknowledgement"></a>
- Hat tip to anyone whose code was used
- Inspiration
- References
