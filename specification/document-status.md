# Document Statuses

Specification documents (files) MAY explicitly define a "Status". If they do,
they MUST display a status immediately after the document title. When present,
the "Status" applies to the individual document only and not to the entire
specification or any other documents. The following table describes what the
statuses mean.

## Lifecycle status

The support guarantees and allowed changes are governed by the lifecycle of the
document. Lifecycle stages are defined in the [versioning](versioning.md) document.

|Status              |Explanation|
|--------------------|-----------|
|No explicit "Status"|Equivalent to Experimental.|
|Experimental        |Breaking changes are allowed.|
|Stable              |Breaking changes are no longer allowed. See [stability guarantees](versioning.md) for details.|
|Deprecated          |Changes are no longer allowed, except for editorial changes.|

## Feature freeze

In addition to the statuses above, documents may be marked as `Feature-freeze`.
These documents are not currently accepting new feature requests, to allow the
GDI specification maintainers time to focus on other areas of the specification.
Editorial changes are still accepted. Changes that address production issues
with existing features are still accepted.

Feature freeze is separate from a lifecycle status. The lifecycle represents
the support requirements for the document, feature freeze only indicates the
current focus of the specification community. The feature freeze label may be
applied to a document at any lifecycle stage. By definition, deprecated
documents have a feature freeze in place.

## Mixed

Some documents have individual sections with different statues. These documents
MUST be marked with the status `Mixed` at the top, for clarity. If a document's
status is marked as `Mixed` then it MUST define at least two different statuses
in sections that follow within the document.
