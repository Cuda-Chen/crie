# Crie

Compile-time Trie

## Installation

1. Add the dependency to your `shard.yml`:

   ```yaml
   dependencies:
     crie:
       github: c910335/crie
   ```

2. Run `shards install`

## Usage

```crystal
require "crie"

# Building Trie in Compile-time
Crie << "En aru'din Raszagal"
Crie << ["Khassar de templari", "Zhakul inok"]
Crie.add_suffixes_of("Terrie Khala")

# Searching in Compile-time
Crie.search("En Taro Adun") # => 3
Crie.search("Khala dora") # => 5

# Searching in Running-time
crie = Crie.new
crie.search("Zhara ku'nuul") # => 3
crie.search("Khas ara'shar") # => 4
```

## Contributing

1. Fork it (<https://github.com/c910335/crie/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Contributors

- [Tatsiujin Chin](https://github.com/c910335) - creator and maintainer