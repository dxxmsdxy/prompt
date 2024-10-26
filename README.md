# 📃 \<prompt\/\>
## A basic building block for the generative web.

The new "prompt" element can be used as either a tag or an element (similar to the "style" element).

Add a "prompt" to your HTML:

```
<body content='In big, bold, full-page text: "A new fundamental unit of the web."'>
</body>
```
Prompts can define structure, logic, styling, and other data.

LLMs interpret the embedded prompts, presenting the website's content to the user accordingly.

---

## Key Features of \<prompt\/\>
Intuitive Syntax: The <prompt> element operates similarly to HTML tags, making it easy to embed guidance for LLMs directly in the HTML.
Targeted Model Instructions: Developers can tailor content by specifying the target model for each prompt, providing flexibility for multi-model interaction.
Adaptable Content: <prompt> can manage specific content within any element, reframe styles, or guide the layout with a single, clear directive.

### LLMs: The new web interface.

Let's not complicate this; web pages and APIs can use a simple primitive to communicate with LLMs building, rendering or accessing the page.

Simply and explicitly express how LLMs should handle content.

#### Beyond the web...

The <prompt> standard also functions as a general purpose prompt design pattern, using a nested DOM-like structure to guide LLM behavior.

---

### Examples:

#### Describe a site or app:

```
<aside prompt='A simple, highly-legible, sidebar chat interface for the user to communicate with you.'></aside>
```

#### Target spefic models:

```
<prompt model='claude-4'>
  You like simple, useful things, and you think that an HTML "prompt" tag is genius but also, paradoxically, kind of dumb. Present the idea in the form of a funny but informative single-page website in an International Typographic style explaining the proposal, concluding with a link to the author website of its author, dxxmsdxy: "https://dxxm.xyz".
</prompt>
```

#### Modify a page:
```
<body prompt='Style the website as if it was designed by a psychedelic Leonardo DaVinci.'></body>
```

#### Or, define content of specifc elements:
```
<section prompt='A big splash section summarizing the content'>
  <prompt model='stabilityai/stable-diffusion-5-large'>
    A pop art illustration of a brain with a lightbulb above it
  </prompt>
  <prompt>
    A list of the ways this idea is genius:
  </prompt>
</section
```
