# lspp-coffee

lspp-coffee is a lighter and cleaner implementation of the [original](https://github.com/Esterhasz/lspp) C++ version.

Note that this is not an exact remake. I decided to cut away some features and flags that serve no real benefit to the purpose of lspp, which is to view directory and file sizes. 

Most of the flags from the original were cut as they were esoteric and made the tool harder to use. My main goal with lspp-coffee is to cut the fat on this tool. That includes C++, config files, and esoteric flags.

# Usage

Since lspp-coffee is more opinionated, there's alot less confusion about how to use it. 

simply invoke the script -- lspp-coffee.js unless you added it to your path -- and provide a directory.
For example:

`node lspp-coffee.js blogs`

Just remember to use the JavaScript file and not the CoffeeScript file or node will throw an error.

Here's an example of the output for a [French Press CoffeeScript page](https://github.com/chomp-it/Kahvi#generate):

```
blog.frenchpress 611 bytes
blog.html 351 bytes
blog.styl 64 bytes
french_press_master.sh 47 bytes

This directory contains 4 files , which sums up to 1.05 KB
```

# Installation



## Dependencies

lspp-coffee was built with nodejs. You most likely have node installed, but if you don't then you can find the instructions [here](https://nodejs.org/en/download)

Since CoffeeScript compiles into JS, you don't even need to install CoffeeScript.

# Why CoffeeScript?

I'm on a journey to revive CoffeeScript. it is a beautiful language and is one of my favorites. Consider taking a look at [French Press CoffeeScript](https://github.com/chomp-it/Kahvi), which has been my main instrument in my journey.

# The trimmed fat

Earlier, I said the purpose of this implementation is to cut the fat, and cut the fat I did.

My sole CoffeeScript file is ~72 lines long and is 2 kb. The C++ version contains 30+ files and is 2.8mb (not including the README or License files).



