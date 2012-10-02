# Ligature Symbols
Ligature Symbols is WebFont project to display the symbol with a ligature features.I created this font by using [FontForge](http://fontforge.sourceforge.net/) (open source postscript font editor).
If you want to learn more, you may read [my blog entry](http://d.hatena.ne.jp/kudakurage/20120720/1342749116).
Demo: [http://kudakurage.com/ligature_symbols/](http://kudakurage.com/ligature_symbols/)

## Browser Support
Ligature Symbols works in all major browsers (Chrome, Firefox, Safari, Opera, IE, iOS, Android)

## Sample HTML
    
    <p>Simple use for mailto link.</p>
    <a href="mailto:mail@example.com" class="lsf">mail</a>
    
    <p>Use tha icon with text.</p>
    <a href="http://twitter.com/" class="lsf-icon" title="twitter">Twitter</a>

## Sample CSS
    
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