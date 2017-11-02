# ember-mask-input

This README outlines the details of collaborating on this ember-mask-input addon.

## Installation

```bash
cd your-project-directory
ember install ember-mask-input
```

## Usage
Simple IBAN masked input:
```handlebars
{{ember-mask-input maskType='iban' value='TR625373458726249832302425' }}
```

Simple phone-no masked input:
```handlebars
{{ember-mask-input maskType='phone-no' value='2223334455' }}
```

Simple credit-card masked input:
```handlebars
{{ember-mask-input maskType='credit-card' value='2222333344445555' }}
```

Simple custom masked input:
```handlebars
{{ember-mask-input mask='0000.0000.0000.0000' value='9876987612341234' }}
```

Actioned masked input:
```handlebars
{{ember-mask-input maskType='iban' value=myIban onUpdate=(action 'valueUpdated') }}
<br/>
Updated value: {{updatedValue}}
```

classNames binding masked input:
```handlebars
{{ember-mask-input value='TR625373458726249832302426' maskType='iban' classNames='myclass' }}
<style>
.myclass {
    width: 400px;
    font-weight: bold;
    font-style: italic;
}
</style>
```
