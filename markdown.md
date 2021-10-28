# Basic Syntax
+ Heading: # H1  ## H2  ### H3  #### H4  ##### H5  ###### H6
+ Bold: \*\*bold text\*\* or \_\_bold text\_\_
+ Italic: \*italicized text\* or \_italicized text\_
+ Blockquote: > blockquote
+ Ordered List: 1. First item 2. Second item 3. Third item
+ Unordered List: - First item - Second item - Third item
+ Code: \`code\`
+ Horizontal Rule: ---
+ Link: \[title\](https:\/\/www.example.com)
+ Image: \!\[alt text\](image.jpg)

# Example
```
# H1
## H2
### H3
#### H4
##### H5
###### H6
**bold text**
__bold text__  
*italicized text*  
_italicized text_  
> blockquote
1. First item 
2. Second item 
3. Third item  
- First item
- Second item
- Third item  
At the command prompt, type `nano`.  
---
[title](https://www.example.com)  
![alt text](https://avatars.githubusercontent.com/u/5618262?s=40&v=4)
```
# H1
## H2
### H3
#### H4
##### H5
###### H6
**bold text**  
__bold text__  
*italicized text*  
_italicized text_  
> blockquote
1. First item 
2. Second item 
3. Third item  
- First item
- Second item
- Third item  
At the command prompt, type `nano`.  
---
[title](https://www.example.com)  
![alt text](https://avatars.githubusercontent.com/u/5618262?s=40&v=4)

# Extended Syntax
+ Table  
\| Syntax \| Description \|  
\| ----------- \| ----------- \|  
\| Header \| Title \|  
\| Paragraph \| Text \|
+ Fenced Cold Block  
\`\`\`
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
\`\`\`
+ Footnote  
Here's a sentence with a footnote. [^1]  
[^1]: This is the footnote.
+ Heading ID  
My Great Heading {#custom-id}
+ Definition List  
term  
: definition
+ Strikethrough  
\~\~The world is flat.\~\~
+ Task list  
\- [x] Write the press release  
\- [ ] Update the website  
\- [ ] Contact the media  

# Example
```
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |

\`\`\`
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
\`\`\`

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
	
### My Great Heading {#custom-id}
[Heading IDs](#custom-id)

First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.

~~The world is flat.~~ We now know that the world is round.

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media


Gone camping! :tent: Be back soon.

That is so funny! :joy:
```
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.  
    Indent paragraphs to include them in the footnote.  
    `{ my code }`  
    Add as many paragraphs as you like.
	
### My Great Heading {#custom-id}
[Heading IDs](#custom-id)

First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.

~~The world is flat.~~ We now know that the world is round.

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media


Gone camping! :tent: Be back soon.

That is so funny! :joy: