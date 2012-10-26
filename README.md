This plugin enables folding by section headings in markdown documents.

Thanks to Kana Natsuno for helping me to test drive this code using [vspec][].

## Running the tests

`test/folding.vim` contains tests written in the [vspec][] format. Here are the barebones instructions for executing the tests, assuming that `vspec` and `markdown-folding` plugins are installed as follows:

    .vim/
      bundle/
        vspec/
          bin/
            vspec
        markdown-folding/
          test/
            folding.vim

You can run the tests as follows:

    cd .vim/bundle/markdown-folding
    ../vspec/bin/vspec ../vspec . test/folding.vim

Execute the tests from inside Vim with this quick-and-dirty mapping (assumes working directory to be `.vim/bundle/markdown-folding`):

    nnoremap <leader>r :wa <bar> ! ../vspec/bin/vspec ../vspec/ . test/folding.vim<CR>

[vspec]: https://github.com/kana/vim-vspec
