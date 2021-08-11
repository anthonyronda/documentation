# Attributing

When making a world using assets collected from other sources, always check the license of all associated works. Licensed works may only be distributed as allowed by the license after meeting all of the obligations of the license text. This page helps clarify those obligations, because every license differs.

## Credits Journal Entry

It is recommended to create a Journal Entry called `Credits` at the root of the Journal Entries in the world you are working on. You could either list each attribution on its own line, categorize them by file type or logically into scenes, actors, etc.

This recommendation is _in addition_ to the attribution method required by the content license, _not a replacement_ for the attribution method required by the license.

### Example Journal Entry

Logically sorted:

```html
<h1>Scenes</h1>
<h2>Scene 1</h2>
<p>Credit 1</p>
<p>Credit 2</p>
<h1>Actors</h1>
<h2>Actor 1</h2>
<p>Credit 1</p>
<p>Credit 2</p>
<h1>Items</h1>
<h2>Item 1</h2>
<p>Credit 1</p>
<p>Credit 2</p>
<h1>Journal Entries</h1>
<h2>Journal Entry 1</h2>
<p>Credit 1</p>
<p>Credit 2</p>
<h1>Playlists</h1>
<h2>Playlist 1</h2>
<p>Credit 1</p>
<p>Credit 2</p>
```

Sorted by file type:

```html
<h1>Image Files</h1>
<p>Credit 1</p>
<p>Credit 2</p>
<h1>Audio Files</h1>
<p>Credit 1</p>
<p>Credit 2</p>
```

## Creative Commons

If you are using material licensed under [Creative Commons](https://creativecommons.org/) (a common license used by many artists), according to the terms of the license, you are required to give credit to the original author and indicate if changes were made. Note that **Creative Commons Zero (CC0, CC0 1.0)** does _not require_ attribution, but it is still a nice thing to do.

### Attribution Structure

Let us examine an example attribution:

> **celebration_grayscale.webp**: "[Creative Commons 10th Birthday Celebration San Francisco](https://www.flickr.com/photos/sixteenmilesofstring/8256206923/in/set-72157632200936657)" by [tvol](https://www.flickr.com/photos/sixteenmilesofstring/) is licensed under [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/). / Desaturated, levels adjusted.

A good source attribution answers the following questions:

| Question     | Answer                                                                                                                                             | Description                                                                                                                                                                                                                                              |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **File?**    | celebration_grayscale.webp                                                                                                                         | What file is this source attribution for? In larger projects containing many files with the same name, you could also use the relative path to the file from the project root directory.                                                                 |
| **Title?**   | [Creative Commons 10th Birthday Celebration San Francisco](https://www.flickr.com/photos/sixteenmilesofstring/8256206923/in/set-72157632200936657) | The original title of the work (**optionally**) linked to the source website. If a title is not provided, don't add one.                                                                                                                                 |
| **Author?**  | [tvol](https://www.flickr.com/photos/sixteenmilesofstring/)                                                                                        | Name of the author—written how the author wishes to be attributed, which may not be their real name—(**optionally**) linked to the author's-website. In rare cases, the author may not want to be attributed at all. In this case, don't add the author. |
| **License?** | [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/)                                                                                          | **Optional:** License abbreviation linked to license deed. Only add this if you _know_ what the license of the source work is.                                                                                                                           |
| **Changes?** | Desaturated, levels adjusted.                                                                                                                      | **Optional:** A _brief_ description of how the original work has been changed. Only add this if you have made _changes_ to the file.                                                                                                                     |

### File Format Conversions

Technically converting an image or an audio file to another format (e.g., a PNG image to WebP, or MP3 audio to Ogg) could be considered changing the source file because if doing a bit-for-bit comparison, the files will not be identical. However, in our use case changing the file format is very commonly done and the change is minor, so it shouldn't be too bad to omit the change notice for file format conversions to make the source attributions shorter and easier to read.

### Example Attributions

The Markdown formatting can be used in git repositories. The HTML formatting is provided for use in Foundry VTT journals.

#### Common Use Case

With no changes made to the file and a single author.

> **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author](author's-website) is licensed under [License Abbreviation](link-to-license-deed).

```md
Markdown: **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author](author's-website) is licensed under [License Abbreviation](link-to-license-deed).
HTML: <p><strong>File Name</strong>: "<a href="link-to-source-website-or-file">Source Page Title or File Name</a>" by <a href="author's-website">Author</a> is licensed under <a href="link-to-license-deed">License Abbreviation</a>.</p>
```

#### Multiple Authors

In the case of multiple authors, separate them by commas.

> **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author 1](author-1's-website), [Author 2](author-2's-website) is licensed under [License Abbreviation](link-to-license-deed).

```md
Markdown: **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author 1](author-1's-website), [Author 2](author-2's-website) is licensed under [License Abbreviation](link-to-license-deed).
HTML: <p><strong>File Name</strong>: "<a href="link-to-source-website-or-file">Source Page Title or File Name</a>" by <a href="author 1's website">Author 1</a>, <a href="author 2's website">Author 2</a> is licensed under <a href="link-to-license-deed">License Abbreviation</a>.</p>
```

#### With Changes

If you have made changes to the file, note them at the end of the line, separated with a forward slash (**/**).

> **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author](author's-website) is licensed under [License Abbreviation](link-to-license-deed). / Briefly describe changes you've made.

```md
Markdown: **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author](author's-website) is licensed under [License Abbreviation](link-to-license-deed). / Briefly describe changes you've made.
HTML: <p><strong>File Name</strong>: "<a href="link-to-source-website-or-file">Source Page Title or File Name</a>" by <a href="author's-website">Author</a> is licensed under <a href="link-to-license-deed">License Abbreviation</a>. / Briefly describe changes you've made.</p>
```

### Table of Creative Commons Licenses

This table is provided for quick reference purposes. For an up to date list of Creative Commons licenses see: [https://creativecommons.org/licenses/](https://creativecommons.org/licenses/)

The table only lists the newer 3.0 and 4.0 versions of the licenses. For all versions, see the [License Versions](https://wiki.creativecommons.org/wiki/License_Versions#Licenses) article on the Creative Commons wiki or simply change the version number in the URL. (E.g., `https://creativecommons.org/licenses/by/4.0/` to `https://creativecommons.org/licenses/by/2.0/`.)

If the content you are attributing does not specify the version of the Creative Commons license (e.g., "licensed under CC-BY"), you can assume it refers to the newest version of the license (**4.0** at the time of writing of this article).

| Title                                                     | Abbr.           | Link                                                       |
| :-------------------------------------------------------- | :-------------- | :--------------------------------------------------------- |
| Attribution 4.0 International                             | CC BY 4.0       | [Deed](https://creativecommons.org/licenses/by/4.0/)       |
| Attribution-ShareAlike 4.0 International                  | CC BY-SA 4.0    | [Deed](https://creativecommons.org/licenses/by-sa/4.0/)    |
| Attribution-NoDerivatives 4.0 International               | CC BY-ND 4.0    | [Deed](https://creativecommons.org/licenses/by-nd/4.0/)    |
| Attribution-NonCommercial 4.0 International               | CC BY-NC 4.0    | [Deed](https://creativecommons.org/licenses/by-nc/4.0/)    |
| Attribution-NonCommercial-ShareAlike 4.0 International    | CC BY-NC-SA 4.0 | [Deed](https://creativecommons.org/licenses/by-nc-sa/4.0/) |
| Attribution-NonCommercial-NoDerivatives 4.0 International | CC BY-NC-ND 4.0 | [Deed](https://creativecommons.org/licenses/by-nc-nd/4.0/) |
| Attribution 3.0 Unported                                  | CC BY 3.0       | [Deed](https://creativecommons.org/licenses/by/3.0/)       |
| Attribution-ShareAlike 3.0 Unported                       | CC BY-SA 3.0    | [Deed](https://creativecommons.org/licenses/by-sa/3.0/)    |
| Attribution-NoDerivs 3.0 Unported                         | CC BY-ND 3.0    | [Deed](https://creativecommons.org/licenses/by-nd/3.0/)    |
| Attribution-NonCommercial 3.0 Unported                    | CC BY-NC 3.0    | [Deed](https://creativecommons.org/licenses/by-nc/3.0/)    |
| Attribution-NonCommercial-ShareAlike 3.0 Unported         | CC BY-NC-SA 3.0 | [Deed](https://creativecommons.org/licenses/by-nc-sa/3.0/) |
| Attribution-NonCommercial-NoDerivs 3.0 Unported           | CC BY-NC-ND 3.0 | [Deed](https://creativecommons.org/licenses/by-nc-nd/3.0/) |
| CC0 1.0 Universal                                         | CC0 1.0         | [Deed](https://creativecommons.org/publicdomain/zero/1.0/) |

For further clarifications about the licenses, see the [License Versions](https://wiki.creativecommons.org/wiki/License_Versions) article on the Creative Commons wiki.

## Open Game License

There are thousands of Dungeons & Dragons and Pathfinder publications available for reuse and redistribtion under the OGL, the same license as the D&D/PF Systems Reference Documents for those systems (SRDs). If one uses and distributes an OGL derivative work, that work must also be OGL licensed. This is similar to a weak copyleft source code license.

Please note that citations for the below are currently being compiled from Wayback Machine backups of the Open Game Foundation's mailing list archive (and other sources). Each paragraph will have a source link on a later date.

### Product Identity and Open Game Content

Every OGL publication should have a section designating portions as Product Identity and portions as Open Game Content. As described in the license text, Open Game Content is the only content that may be reused. If this section is missing, one should confirm with the publisher which portions are Open Game Content. The license is written such that the entire publication is Open Game Content if nothing is explicitly declared, though it is safest to ask before reusing the publication.

The Open Game License only grants reuse under copyright law, and does not grant a license for trademark or patent use.

#### Declaring Product Identity and Open Game Content in Your Package

One must remove all Product Identity one doesn't have explicit permission to use, and must not include it in their OGL derivative work. One may include new content (content for which one owns the copyright) in their derivative work and declare it as Product Identity.

If this is desired, include the phrase `Product Identity:` followed by a detailed description of the content or the location of the content that is not Open Game Content. Otherwise everything included will be considered Open Game Content. If something in the package is licensed under a separate license and should not be licensed under OGL, declare it as Product Identity.

Also include the phrase `Open Game Content:` in a separate paragraph, followed by a detailed description of the content or the location of the content that _is_ Open Game Content. For the most clarity, both of these paragraphs together should describe _all_ of the copyrighted content in your package.

### The OGL 1.0a License Text

This wiki recommends two versions of the license text for your use.

- [OGL 1.0a with linebreaks](https://raw.githubusercontent.com/anthonyronda/LicenseRef-OGL-1.0a/main/LICENSE) for viewing in text editors without word wrap
- [OGL 1.0a without linebreaks](https://raw.githubusercontent.com/anthonyronda/LicenseRef-OGL-1.0a/open-gaming-foundation-without-line-breaks/LICENSE) for use in documents with word wrap

One should use the version that suits one's usecase. Capitalization and punctuation may not match the original works that the package is reusing; this is fine (they often don't match each other either). These text files are a match to an upcoming [SPDX](https://spdx.dev) proposal, which will allow them to be used by license compliance tools.

#### Preparing an OGL License Text For Your Package

At the end of the provided OGL text, one must include the proper copyright notices.

First, the copyright notice for the license itself is always included in the text as the first copyright notice.

`Open Game License v 1.0a Copyright 2000, Wizards of the Coast, Inc.`

Next, Each on their own lines, create a copyright notice for each work being reused, and each work cited in that work's COPYRIGHT NOTICE section, including publication title, publication year, and publication author(s) just like in the original copyright notice.

Finally, include the package title, package publication year, and package author(s) as the final copyright notice.

#### Preparing Multiple OGL License Texts For Your Package

Including Open Game Content from multiple OGL publications in the same package can make the COPYRIGHT NOTICE section unwieldy to read, though it is allowed. It also makes reuse more complicated, since users won't know which Open Game Content came from which publications. Another option is to prepare multiple license texts for individual portions of world content.

To do this, each OGL license text should be included in a subdirectory that contains a specific portion of Open Game Content. Each license text would therefore have different copyright notices depending on what content is contained in that subdirectory. This makes the reading the copyright notices and reusing specific portions of the content far easier.

### Including the License Text in your Work

The prepared license text(s) should be distributed in the package for easy viewing by any user of the content. Because the license text may change as you provide updates to your package, it's advisable _not_ to store the text in a Journal Entry in addition to a text file, where mistakes could lead to them being out of sync. Instead, link to the file in a Journal Entry, or find some other manner in which OGL text can be accessed via the application.

## Unknown License

If the source material license is unknown, but you still want to credit the author.

> **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author](author's-website).

```md
Markdown: **File Name**: "[Source Page Title or File Name](link-to-source-website-or-file)" by [Author](author's-website).
HTML: <p><strong>File Name</strong>: "<a href="link-to-source-website-or-file">Source Page Title or File Name</a>".</p>
```

---

Portions of this guide are loosely based on the "[Best practices for attribution](https://wiki.creativecommons.org/wiki/Best_practices_for_attribution)" article on the Creative Commons wiki, licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
