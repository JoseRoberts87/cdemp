## CDEMP for Stylus
Component Definitions Element Modifiers and Properties is methodology for creating componetized frontend assets the purpose of which is to encourage code reuse and, ultimately leading to more efficient stylesheets that are easier to add to, read, and maintain.

## Installation
```
git clone https://github.com/amansx/cdemp cdemp
```

## Usage
### Components
A component is an identifiable part of a larger application and provides a particular function or group of related functions to given markup element.
#### Stylus
```css
{DEF_CMP}_COMPONENT-NAME{
	height: 100px;
}
```
#### HTML
```
<div class="cmp_COMPONENT-NAME">
</div>
```
## Elements
#### Stylus
```css
{DEF_CMP}_COMPONENT-NAME{
	height: 100px;
	
	{DEF_EL}_title{
		color: black;
	}
}
```
#### HTML
```
<div class="cmp_COMPONENT-NAME">
	<span class="cmp_COMPONENT-NAME_title"> Title </span>
</div>
```
## Properties
#### Stylus
```css
{DEF_CMP}_COMPONENT-NAME{
	height: 100px;
	
	{DEF_PROP}_color{
		{DEF_VAL}--blue{
			color: blue;
		}
	}
}
```
#### HTML
```
<div class="cmp_COMPONENT-NAME p_color--blue">
	<span class="cmp_COMPONENT-NAME_title"> Title </span>
</div>
```
## Modifiers
#### Stylus
```css
{DEF_MODIFIER}-default-font{
	use_font("default");
}
```
#### HTML
```
<div class="cmp_COMPONENT-NAME use-default-font">
	...
</div>
```
## Boolean
#### Stylus
```css
{DEF_CMP}_COMPONENT-NAME{
	height: 100px;
	
	{DEF_BOOL}-themed{
		load_theme();
	}
}
```
#### HTML
```
<div class="cmp_COMPONENT-NAME is-themed">
	...
</div>
```


