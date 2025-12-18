# Imgy Tagger

Bulk tag images before uploading to Canva on desktop / mobile with keywords using XMP Standard, it works offline (Made with help of various AI tools).

> Try: https://imgytagger.netlify.app/


## The idea  :

Every image has metadata, it's a set of information tells you when the image was taken, where it was taken, what kind of camera or phone made it... etc.
We can use keywords (tags) inside image's metadata to identify and organize images.

That's where this tool comes in, it uses the Extensible Metadata Platform (XMP) Standard to embed descriptive tags into the `dc:subject` field of an image's metadata.
<p align="center">
<img width="900" height="508" alt="1" src="https://github.com/user-attachments/assets/af1a3554-9a0a-4e6a-bf83-fc00d429c243" />
<br><br>
<img width="900" height="508" alt="2" src="https://github.com/user-attachments/assets/882a9036-295e-48ac-8d6c-cbc7a6d7bf02" />
</p>

---

To make sure that the tags you made are embedded, after uploading your tagged images to Canva, click the three dots on any image to view its details. You’ll find your custom tags listed under the `"Manual tags"` section. These tags can then be used to search and retrieve all images that share the same keywords.
<p align="center">
<img width="900" height="508" alt="3" src="https://github.com/user-attachments/assets/35d9954a-a48a-4357-9641-000f9aef6709" />
<br><br>
<img width="900" height="508" alt="4" src="https://github.com/user-attachments/assets/a245fcbe-cac3-4b8d-a0f3-3300cba2a2a0" />
</p>

**It's completely offline** tool working on client-side (your browser) without sending any data to the server, and working on Desktop/Mobile.  
In other words, if you loaded the website and saved the page locally as an HTML file, you can open the HTML file from your device and do your work without needing to visit the website (or simply download with [ctrl+shift+s](https://github.com/abdo2048/imgyTagger/blob/main/ImgyTagger.html)). 

## Is it limited to Canva?
No, once you tag and save your images, you have the possibility to organize them with any online/offline software that supports viewing image's XMP metadata. it's just the birth of tool comes from not being able to bulk tag images on Canva, whether while uploading images or after.

## Features:
- **Embeds Tags in XMP Metadata**  
Uses the XMP standard (via `dc:subject`) for broad format support, including PNG and JPEG—unlike EXIF.
- **Fully Offline & Private**  
No internet required. All processing happens locally in your browser.
- **Cross-Platform & Responsive**  
Works seamlessly on desktop and mobile devices (see note 2), across Chrome, Firefox, Edge.
- **Smart Duplicate Prevention**  
Blocks duplicate uploads using file names and hash-based fingerprinting.
- **Flexible Selection & Batch Actions**  
Select all , deselect, or invert image selections. Apply or reset tags in bulk.
- **Grid & List Views with Zoom**  
Toggle between views and adjust grid size with a zoom slider (visual only).
- **Tag Reuse & History**  
Auto-suggests previously used tags as you type for consistency and speed.
- **Tag Management**  
Add new tags or merge them with existing ones on already-tagged images.  
Reset tags anytime—before or after download—and re-tag freely.

## Notes / Thoughts:
- Try to be picky while tagging images, because using general tags only like `"nature"` for example, will bring more image results while searching in Canva, since it has its own AI (smart) tags.
- When downloading multiple images, it's recommended to disable (if not already disabled by default) the **"Ask where to save each file before downloading"** setting in your browser settings, so that it won't gives you multiple prompts asking you where to download each image.
- When using imgy Tagger on mobile, **avoid selecting images directly from the gallery picker.** Instead, tap the three dots in the picker and choose "Browser" to open your file manager, then select images from there. This preserves the original filenames—choosing directly from the gallery may rename them to random numbers. Also note that some browsers might prevent multiple downloads.
- **Canva can read existing image tags but doesn't embed new ones.** If you add or edit tags in Canva (the manual tags section), **those changes only apply within the Canva platform**—they won’t be saved into the image’s metadata. So, if you download the image from Canva after editing tags, and loaded it to this tool or other metadata tools, the tags won’t appear because Canva doesn’t embed them in the file.
- There are things that might needs to changes/enhanced regarding user interface or functionality, but I guess the tool is usable at this point. **If you are wants to help / improve or build upon the tool, I encourage you to do that.**
