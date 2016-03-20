# F# RFC FS-1010 - Add Map.count

The design suggestion [Add Map.count](https://fslang.uservoice.com/forums/245727-f-language/suggestions/12880398-add-map-count) has been marked "approved in principle".
This RFC covers the detailed proposal for this suggestion.

* [ ] Details: [under discussion](https://github.com/fsharp/FSharpLangDesign/issues/78)
* [ ] Implementation: [In progress](https://github.com/Microsoft/visualfsharp/pull/1007)


# Summary
[summary]: #summary

Add ``Map.count``.  

# Motivation
[motivation]: #motivation

This was requested in this uservoice: https://fslang.uservoice.com/forums/245727-f-language/suggestions/12880398-add-map-count

The main motivation is to make the module more regular, it seems strange to me that you should need to use the module for most map operation, but are forced to use instance members for others. I think it's quite similar to the clean up of the Seq/List/Array module collections that was done for F# 4.0, which was requested here: https://fslang.uservoice.com/forums/245727-f-language/suggestions/5663997-make-fsharp-core-collection-functions-for-list-ar 

It's a shame, Set/Map call this concept "count" as Seq/Map/List all call it "length", but I think it's too late to change this.

# Detailed design
[design]: #detailed-design

Very simple design, no need to go into detail here.

# Drawbacks
[drawbacks]: #drawbacks

Note that the instance property ``.Count`` is already available.  The main drawback is that it gives two ways to do the same thing.

# Alternatives
[alternatives]: #alternatives

The alternative is to keep things as they are.

# Unresolved questions
[unresolved]: #unresolved-questions

None
