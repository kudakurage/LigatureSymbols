# Ligature Symbols
Ligature Symbols is WebFont project to display the symbol with a ligature features.I created this font by using [FontForge](http://fontforge.sourceforge.net/) (open source postscript font editor).
IF you want to learn more, you may read [my blog entry](http://d.hatena.ne.jp/kudakurage/20120720/1342749116).
Demo : [http://kudakurage.com/ligature_symbols/](http://kudakurage.com/ligature_symbols/)

## Support Browser
Ligature Symbols has broad support for the modern browser (Chrome, Safari, Firefox, iOS - Mobile Safari, Android Browser).

## Sample HTML & CSS

    <!-- HTML -->
    
    <p>Simple use for mailto link.</p>
    <a href="mailto:mail@example.com" class="lsf">mail</a>
    
    <p>Use tha icon with text.</p>
    <a href="http://twitter.com/" class="lsf-icon" title="twitter">Twitter</a>

    /* CSS */
    
    @font-face {
        font-family: 'LigatureSymbols';
        src: url('LigatureSymbols.eot');
        src: url('LigatureSymbols.eot?#iefix') format('embedded-opentype'),
             url('LigatureSymbols.woff') format('woff'),
             url('LigatureSymbols.ttf') format('truetype'),
             url('LigatureSymbols.svg#LigatureSymbols') format('svg');
        src: url('LigatureSymbols.ttf') format('truetype');
        font-weight: normal;
        font-style: normal;
    }
    
    .lsf, .lsf-icon:before {
        font-family: 'LigatureSymbols';
        -webkit-text-rendering: optimizeLegibility;
           -moz-text-rendering: optimizeLegibility;
            -ms-text-rendering: optimizeLegibility;
             -o-text-rendering: optimizeLegibility;
                text-rendering: optimizeLegibility;
        -webkit-font-smoothing: antialiased;
           -moz-font-smoothing: antialiased;
            -ms-font-smoothing: antialiased;
             -o-font-smoothing: antialiased;
                font-smoothing: antialiased;
    }
    
    .lsf-icon:before {
        content: attr(title);
        margin-right: .3em;
        font-size: 130%;
    }

## License
You can get Ligature Symbols for free.
This Font is licensed under [the SIL Open Font License](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=OFL).
