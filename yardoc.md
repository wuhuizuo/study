study yard notes
=============

##Tags
- @author wuhuizuo
- @deprecated Use {#hello} instead of this method
- @param
- @return
- @note
...
> a list of tags can be found in file:docs/Tag.md#taglist

##Reference Tags
- (see #other_method)
- @param (see #other_method)
- @return (see #other_method)

##Declaring Types
- [String]
- [String, nil]
- [#to_s]
- [true, false]
- [Array<String>]
- [Array<String, Symbol>]
> more types see: [yardoc types](http://yardoc.org/types.html)

##Documenting DSL Methods
- attr serise, for those ones ,you add comment will generate docs
- manully declare a method with @method tag
- @attribute
> - @attribute [w]
> - @attribute [r]
> - @attribute [rw]
- @scope class
- @visibility private

##Macros
- once defined, use repeated
- example:
> # @!macro dm.property
> # @return [$2] the $1 $0 of the post
> property :tile, String
> ....................
> # some other place
> # @macro dm.property
- @macro [attach]

##Customized YARD Markup
- Linking Objects {...}
> {ObjectName#method OPTIONAL_TITLE}
> {Class::CONSTANT My constant's title}
> {#method_inside_current_namespace}
- Note that the @see tag automatically links its data. You should not use the link syntax in this tag:

 > #@see #methodname   <- Correct.
 > #@see {#methodname} <- Incorrect.
- Linking URLs
  > {url, title}
  > {file:file_path}
- Embedding Docstrings
> # {include: file_path}
> # {include:file:...}
> # {include:file:...}
- Rendering Object {render:...}













