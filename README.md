# llvm_toy_language
showing how to implement a simple language using LLVM components in C++.

Install llvm using brew and extract the path and set the environment. 

<code>
echo 'export PATH="/opt/homebrew/opt/llvm/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
</code>


clang++ -g -O3 my_lang.cpp `llvm-config --cxxflags --ldflags --system-libs --libs core`  -o my_lang