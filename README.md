Pottery - A CSS Framwork in CLay Haskell
=======

We have developed fuctional libraries for automatic generation of CSS using popular design paradigms.  For this we ha have used Clay which is a CSS preprocessor like LESS and Sass, but implemented as an embedded domain specific language (EDSL) in Haskell. This means that all CSS selectors and style rules are first class Haskell functions, which makes reuse and composability easy. We have developed two libraries using Vertical Rhythm design paradigm and Golden Ration design paradigm in this project.

**VERTICAL RHYTHM**

**CONCEPT**

In design, vertical rhythm is the structure that guides a reader’s eye through the content.
Good vertical rhythm makes a layout more balanced and beautiful and its content more
readable. There are 3 primary factors governing rhythm in a document- the font size, line
height and margin or padding. All of these factors must calculated with care in order that
the rhythm is maintained. The basic unit of vertical space is line height. Establishing a
suitable line height that can be applied to all text on the page is the key to a solid
dependable vertical rhythm, which will engage and guide the reader down the page.

**OUR IMPLEMENTATION-**

**Configurable Variables**- Base Font Size, Base Line Height, Rhythm Border Style, Relative Font Sizing, Round To Nearest Half Line, Font Unit.

**Mixins Include-**

o establishBaseline : Establishes the baseline for the given CSSState

o Baseline : Returns baseline CSS

o Rhythm : Calculate rhythm units

o toFontSize: changes fontsize

o fontSize : returns Css to adjust Fontsize of a element

o linesToFontSize : Calculate the minimum multiple of rhythm units needed to contain the font-size.

o Leader : Apply leading whitespace. The property can be margin or padding. By default property is margin.

o paddingLeader : Apply leading whitespace as padding.

o paddingTrailer : Apply trailing whitespace as padding.

o marginLeader : Apply leading whitespace as margin.

o Trailer : Apply trailing whitespace. The property can be margin or padding. By default property is margin.

o marginTrailer : Apply trailing whitespace as margin.

o propertyRhythm : Shorthand function to apply whitespace for top and bottom margins and padding. Takes the number of lines for each property with default value 0.

o applySideRhythmBorder : Apply a border & whitespace to any side without destroying the vertical rhythm. The whitespace must be greater than the width of the border.

o rhythmBorders : Apply borders and whitespace equally to all sides.

o leadingBorder : Apply a leading border.

trailingBorder : Apply a trailing border.

horizontalBorder : Apply both leading border and trailing border

hBorder : Alias for horizontal-border.




**GOLDEN RATIO**

**CONCEPT**

When designing the visual aspect to a website or creating images in general the dilemma of
choosing proportions inevitably comes up. The Golden Ratio or ‘φ’ which equals 1.618 in
decimal terms helps to solve this. The Golden Ratio and the Golden Rectangle is used in
many forms of art and design. In the Renaissance period, many artists proportioned their
artworks according to this ratio and rectangle. In ancient Greece, architects used this
rectangle in the design of the buildings; the Parthenon is a good example of this. Even in
modern architecture, the golden rectangle has a strong presence. Even in modern web
design, the Golden ratio has proven its worth for aesthetics.

**OUR IMPLEMENTATION**

**Mixins Include-**

grTitleSize - Returns CSS of title size based on content width.

grHeadlineSize - Returns CSS of headline size based on content width.

grSubHeadlineSize - Returns CSS of subheadline size based on content width.

grFontSize - Returns CSS of Font size based on content width.

grSecondaryText - Returns CSS of Secondary Text based on content width.

grBaseLineheight : Returns CSS of default line-height based on content width.

grCustomLineheight : Returns CSS of Golden-ratio line-height based on a customvalue specified by the user.
