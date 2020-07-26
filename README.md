# Digilent Infobox for Dokuwiki

The Infobox plugin for Dokuwiki provides easy to use syntax for
creating infoboxes in Dokuwiki.
### Installation

------------------------------------------------------------------------

Clone from [github](https://github.com/Digilent/dokuwiki-infobox) into `$dokuwiki/lib/plugins/infobox.`

### Syntax {#syntax .sectionedit3}

------------------------------------------------------------------------

Invoke the Infobox plugin using:

```
{{Infobox
|
}}
```

Start each new line with a **|** (pipe) character and one of the
following items:

**Title**

Sets the title at the top of the infobox.

```
| Title = <Title Text>
```

**Header**

Inserts a full row header.

```
| Header = <Header Text>
```

**Full Row**

Inserts a full row. Basic wiki syntax is allowed inside the row.

```
| Full Row = <Wiki Markup>
```


**Name = Value**

Inserts a two column name value pair.

```
| <Name> = <Value>
```

**Bullet**

Inserts a full row starting with a bullet.

```
| Bullet = <Bullet Text>
```


### Examples

------------------------------------------------------------------------

```
{{Infobox
| Title = Example Title
| Full Row = Example Full Row
| Header = Example Header 1
| Name = Value
| Name 2 = Value 2
| Name 3 = [[# | Link Example]]
| Header = Header 2
| Bullet = Some bulleted text
| Bullet = In List Form
}}
```
```html
<div class="infobox">
<div class="infobox-table">
<div class="infobox-title">
Example Title
</div>
<div class="infobox-subtitle">
</div>
<div class="section">
<div class="full-row">
Example Full Row
</div>
</div>
<div class="section">
<div class="section-header">
Example Header 1
</div>
<div class="key-value">
<div class="key">
Name
</div>
<div class="value">
Value
</div>
</div>
<div class="key-value">
<div class="key">
Name 2
</div>
<div class="value">
Value 2
</div>
</div>
<div class="key-value">
<div class="key">
Name 3
</div>
<div class="value">
<a href="https://reference.digilentinc.com/reference/software/dokuwiki/infobox" class="wikilink2" title="reference:software:dokuwiki:infobox" rel="nofollow"> Link Example</a>
</div>
</div>
</div>
<div class="section">
<div class="section-header">
Header 2
</div>
<div class="bullet-row">
<ul class="bullet-ul">
<li class="bullet-li">
Some bulleted text
</li>
</ul>
</div>
<div class="bullet-row">
<ul class="bullet-ul">
<li class="bullet-li">
In List Form
</li>
</ul>
</div>
</div>
</div> 
</div>
```
