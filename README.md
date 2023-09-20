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
![image](https://github.com/SivaLutalica/github-docs-example/assets/2844387/803700e5-7d87-466a-8d1d-0951b905dfb9)

Please use also codeblocks for displaying Errors that appear in console.

```bash
Traceback (most recent call last):
        2: from /usr/bin/irb:23:in `<main>'
        1: from (irb):1
RuntimeError: This is a custom error message
```
> Here is an example of using codeblock to display colorcoded bash Error"

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

## References

- [Basic writing and formatting syntax (GitHub Flavored Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup>[1]</sup>
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)<sup>[2]</sup>
- [GitHub Flavored Markdown (Task Lists)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists)<sup>[3]</sup>
- [GFM Emoji CheatSheet](https://github.com/ikatyang/emoji-cheat-sheet)<sup>[4]</sup>
- [GFM - Tables](https://github.github.com/gfm/#tables-extension-)<sup>[5]</sup>
