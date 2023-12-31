# Github Docs Example

## Step 1 - Using Codeblocks

Codebloks in markdown make it *very easy* for people to **copy, paste, share** code.
A good **Cloud Engineer** use Codeblocks whenever possible.

It allows other to copy and read code more easily.

- In order to create codeblocks use backticks `
- Not to be confused with single quote '

```
def find_missing(sequence)
  consecutive     = sequence.each_cons(2)
  differences     = consecutive.map { |a,b| b - a }
  sequence        = differences.max_by { |n| differences.count(n) }
  missing_between = consecutive.find { |a,b| (b - a) != sequence }
  missing_between.first + sequence
end
find_missing([2,4,6,10])
# 8
```
- When you can you can apply snytax highligting to your codeblocks

```Ruby
def find_missing(sequence)
  consecutive     = sequence.each_cons(2)
  differences     = consecutive.map { |a,b| b - a }
  sequence        = differences.max_by { |n| differences.count(n) }
  missing_between = consecutive.find { |a,b| (b - a) != sequence }
  missing_between.first + sequence
end
find_missing([2,4,6,10])
# 8
```
![image](https://github.com/SivaLutalica/github-docs-example/blob/main/assets/269402479-803700e5-7d87-466a-8d1d-0951b905dfb9.png)

Please use also codeblocks for displaying Errors that appear in console.

```bash
Traceback (most recent call last):
        2: from /usr/bin/irb:23:in `<main>'
        1: from (irb):1
RuntimeError: This is a custom error message
```
> Here is an example of using codeblock to display colorcoded bash Error"

## Step 2 - How to take screenshots

A screenshot is when you capture screen of your display using a tool suche as Snippng tool

This is not to be confused with thaking photo with your phone

****DONT DO THIS****

![Phone Photo](assets/phone-photo.jpg)

****DO DO THIS INSTEAD****

![Screenshot](assets/Screenshot%202023-09-20%20225115.png)

**For macOS:**

1. **Entire Screen:**
  - Press Command (⌘) + Shift + 3
  - The screenshot will be saved to your desktop by default.

2. **Selected Portion:**
  - Press Command (⌘) + Shift + 4
  - Drag to select the area of the screen you want to capture.
  - The screenshot will be saved to your desktop by default.

3. **Capture a Window:**
  - Press Command (⌘) + Shift + 4, then press Spacebar.
  - Click on the window you want to capture.
  - The screenshot will be saved to your desktop by default.

4. **Capture Touch Bar (if you have one):**
  - Press Command (⌘) + Shift + 6
  - The screenshot will be saved to your desktop by default.

**For Windows:**

1. **Entire Screen:**
  - Press PrtScn (Print Screen) key.
  - The screenshot is copied to the clipboard. You can paste it into an application like Paint or Word.

2. **Active Window:**
  - Press Alt + PrtScn
  - The screenshot of the active window is copied to the clipboard. You can paste it into an application.

3. **Selected Portion using Snip & Sketch (available in recent Windows versions):**
  - Press Windows + Shift + S
  - Your screen will dim, and you can select an area to capture.
  - The screenshot is copied to the clipboard. You can paste it into an application.

4. **Using Snipping Tool (available in older Windows versions):**
  - Search for "Snipping Tool" in the start menu.
  - Open the application and click on "New" to take a screenshot.
  - Save the screenshot.

For both operating systems, there are also third-party applications available that offer more advanced screenshot functionalities, but the above methods are built-in and don't require additional software.

## Step 3 - Use GitHub Flavoured Markdown Task Lists

GitHub extends Markdown to have lists where you can check off items.
- [x] Finish step 1
- [ ] Finish step 2
- [ ] Finish step 3

## Step 4 - Use emojis

GitHub Flavoured Markdown (GFM) supports emoji short codes here are some examples
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: | 
| Cloud with lightning | `:cloud_with_lightning:` | :cloud_with_lightning: | 

## Step 4 - How to create table

You can use the following to create table

```md
| Name | Shortcode | Emoji |
| --- | --- | --- |
| Cloud | `:cloud:` | :cloud: | 
| Cloud with lightning | `:cloud_with_lightning:` | :cloud_with_lightning: | 
```
GitHub extends the functionality of Markdown tables to provide more alignment and table cell formatting options. [<sup>[5]</sup>](#references)

![Pipe key example](assets/Grammarist-Article-Graphic-V2-58-1024x478.png)

[Secret Window Hidden Garden](secret-window/hidden-garden.md)
## References

- [Basic writing and formatting syntax (GitHub Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup>[1]</sup>
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)<sup>[2]</sup>
- [GitHub Flavored Markdown (Task Lists)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)<sup>[3]</sup>
- [GFM Emoji CheatSheet](https://github.com/ikatyang/emoji-cheat-sheet)<sup>[4]</sup>
- [GFM - Tables](https://github.github.com/gfm/#tables-extension-)<sup>[5]</sup>
