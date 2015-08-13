# assertive.data

A set of predicates and assertions for checking the properties of (country independent) complex data types.  Most of the documentation is on the *[assertive](https://bitbucket.org/richierocks/assertive)* page.  End-users will usually want to use *assertive* directly.


### Installation

To install the stable version, type:

```{r}
install.packages("assertive.data")
```

To install the development version, you first need the *devtools* package.

```{r}
install.packages("devtools")
```

Then you can install the *assertive.data* package using

```{r}
library(devtools)
install_bitbucket("richierocks/assertive.data")
```

### Predicates

`is_cas_number` checks character vectors for Chemical Abstracts Service registry
numbers.

`is_credit_card_number` checks character vectors for credit card numbers.

`is_email_address` checks character vectors 

`is_hex_color` (and its synonym, `is_hex_colour`) check character vectors for
hexadecimal colors.

`is_honorific` checks character vectors for honorifcs, like Mr and Mrs.

`is_ip_address` checks character vectors for Internet Protocol addresses.

`is_isbn_code` checks character vectors for International Standard Book Numbers.
`is_isbn10_code` and `is_isbn13_code` check only for the 10/13 digit ISBNs.

### Assertions

Predicates all return a vector and have two corresponding assertions.  For example,
`is_cas_number` has `assert_all_are_cas_numbers` and `assert_any_are_cas_numbers`.
