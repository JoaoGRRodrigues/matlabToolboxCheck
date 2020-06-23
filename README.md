# matlabToolboxCheck
MATLAB function to check whether native toolboxes have licenses available and are installed.

Developers can integrate this function into their scripts to quickly verify that users have the required toolboxes to run their scripts and if not, warn users.

General users can also use this to quickly get a table of all available MATLAB features or toolboxes along with both their program and human-readable (marketing) names.

Contact: __Biafra Ahanonu, PhD (bahanonu [at] alum [dot] mit [dot] edu)__.

Made in USA.<br>
<img src="https://user-images.githubusercontent.com/5241605/71493809-322a5400-27ff-11ea-9b2d-52ff20b5f332.png" align="center" title="USA" alt="USA" width="auto" height="50">

## Installation

Download or clone the `matlabToolboxCheck` repository and place the root folder in the MATLAB path. Follow instructions for use below.

Also find function on MATLAB File Exchange: [![View matlabToolboxCheck on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/77275-matlabtoolboxcheck).

## Usage

```MATLAB
% Run with defaults (e.g. toolboxList and secondaryToolboxList options).
[outputTable] = matlabToolboxCheck();

% Check for specific toolboxes requested by user.
[outputTable] = matlabToolboxCheck('toolboxList',{'distrib_computing_toolbox','image_toolbox'},'secondaryToolboxList',{});

% [Alternative] Check for specific toolboxes requested by user.
[outputTable] = matlabToolboxCheck('toolboxList',{'Parallel Computing Toolbox','Image Processing Toolbox'},'secondaryToolboxList',{});

% Run giving out a table of all MATLAB toolboxes/features along with license availability and install status.
[outputTable] = matlabToolboxCheck('dispType','all');

```

## License

See `LICENSE`. MIT @ Biafra Ahanonu