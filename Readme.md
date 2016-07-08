# Solr Indexing Plugin for Discourse

Very simple plugin to index new posts and automatically reindex the entire message board on a provided Solr instance.

The provided serializer supports the excellent 'Discourse Translator' plugin for multi-lingual posts.
This is currently designed to be eventually consistant, picking up languages and translations when new
posts are added to a Topic or at every full reindex.

## How to use

 - Clone and modify the Serializer class in plugin.rb to match your search index fields.
 - [Add your modified plugin][1] to your Discourse instance and restart
 - Set the Solr indexing server address on the Discourse plugin administration page
 - Enable the Solr Indexing plugin

[1]: https://meta.discourse.org/t/install-a-plugin/19157