# HTML Entities JS

A small class to encode and decode the most common HTML entities in a given string.

The class takes great care to ensure that the characters are encoded and decoded in the correct order to avoid character duplication.

See it in action on [JsFiddle][jsfiddle]

## Usage:

	var text = '"&\'<> ¡¢£¤¥¦§¨©ª«¬®¯°±²³´µ¶·¸¹º»¼½¾¿ÀÁÂÃÄÅÆÇÈÉÊËÌÍÎÏÐÑÒÓÔÕÖ×ØÙÚÛÜÝÞßàáâãäåæçèéêëìíîïðñòóôõö÷øùúûüýþÿŒœŠšŸƒˆ˜ΑΒΓΔΕΖΗΘΙΚΛΜΝΞΟΠΡΣΤΥΦΧΨΩαβγδεζηθικλμνξοπρςστυφχψωϑϒϖ–—‘’‚“”„†‡•…‰′″‹›‾⁄€ℑ℘ℜ™ℵ←↑→↓↔↵⇐⇑⇒⇓⇔∀∂∃∅∇∈∉∋∏∑−∗√∝∞∠∧∨∩∪∫∴∼≅≈≠≡≤≥⊂⊃⊄⊆⊇⊕⊗⊥⋅⌈⌉⌊⌋⟨⟩◊♠♣♥♦';

	var encoded = HtmlEntities.encode(text);
	var decoded = HtmlEntities.dencode(encoded);

	// Get the character and entity map
	var map = HtmlEntities.map;

## REFERENCES

The current entity reference is here: [elizabethcastro.com][current].
Although I'm not sure when, it would be preferred to update to use [W3C][next].

However, the most common entities are addressed.

[current]: http://www.elizabethcastro.com/html/extras/entities.html
[next]: http://dev.w3.org/html5/html-author/charref
[jsfiddle]: https://jsfiddle.net/BideoWego/muuvvof8/