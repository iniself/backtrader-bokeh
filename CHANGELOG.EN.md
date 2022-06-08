# Changelog
All notable changes to this project will be documented in this file. Please refer to the [project wiki](https://github.com/iniself/backtrader_bokeh/wiki) for detail.

Telegram Channel: [Aui_Say](https://t.me/aui_say)

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
- More, waiting for update

## [0.1.2] - 2022.06.08
### Commit Hash
- e37eb7bd32058815c20cb048d802268cf0b89fae

### Added
- None

### Fixes
- None

### Changed
- Set the default values of some options as follows, so that users can get the same result with fewer parameters
    * Change the default dark theme to the default light theme
    * `autostart` default is `True`. You no longer need to pass in `autostart` to automatically open the browser
    * `force_plot_legend` default is `True`。You no longer need to pass in `force_plot_legend` to automatically fix the legend bug

## [0.1.1] - 2022.06.08
### Commit Hash
- a27dd6aea434922d681005d72d70ffc55eb050de

### Added
- None

### Fixes
- None

### Changed
- Modify html style
- Update doc

## [0.1.0] - 2022.05.31
### Commit Hash
- 987bc8fa634ce8e4513d993493ab30be980a39d6

### Added
- Add resources option
- More analyzers can be displayed in Analyzers Tab

### Fixes
- Fix lots of bug

### Changed
- Update wiki

## [0.1.0] - 2022.05.23
### Commit Hash
- bcc19c0c0268e87bedcd31f1fe5d966b9743a155

### Added
- Can set special transaction rules
- Add more content of order when printing

### Fixes  
- Fix lots of bug

### Changed
- Modify rendered HTML
- Update wiki

## [0.0.9] - 2022.05.13
### Commit Hash
- 45bd077ba5d474fd36ac5336f6e8209bcb415744

### Added
- In addition to OHLC, additional datafeed line can be plotted

### Fixes  
- None

### Changed
- None

## [0.0.8] - 2022.05.08
### Commit Hash
- e8af78183190190c1e6a19b6ab9380115b1bda3b

### Added
- Fix many bugs of Backtrader through Backtrader_Bokeh's patch, instead of modifying the source code of backtrader

### Fixes  
- fix `autostart` bug in **Live Mode**
- Other bug

### Changed
- A set of easier and clearer Api 
- Update all demo according to new api
- Update README.md
- Update wiki homepage include **en** and **cn**

## [0.0.7] - 2022.05.02
### Commit Hash
- e481f4d7972203e359999a7f6e3d76733788218f

### Added
- Can customize the style of each data. Besides passing in the `style`  like `BacktraderBokeh(style='bar')` , you can do the following
    ```
    data = bt.feeds.YahooFinanceCSVData(
        ...
    )
    data.plotinfo.plotstyle = 'bar'    
    ```

### Fixes  
- fix : TypeError: unhashable type: 'slice' for pandas

### Changed
- None

## [0.0.6] - 2022.04.13
### Commit Hash
- e3b4bff790dfb7216409a552baf7ea3e8f2ffe26

### Added
- In live mode,  the option `autostart = True`  can open the browser automatically

### Fixes  
- Fixed hover-tooltips bug: now, more data lines can be added exactly using the scheme option hover_tooltip_config!

### Changed
- Update README.md and CHANGELOG.md

## [0.0.5] - 2022.04.10
### Commit Hash
- e11863504b7948c2bb9743313ba66279eedf2031

### Added
- None

### Changed
- None

### Removed
- None
  
### Fixes
- Because of optbrowser address and port assignment mistake problem, if port 80 is occupied, the web page will not be opened in the optimization mode
- Very imortant, fixed the legend can't be displayed in the observer or indicators's figuer