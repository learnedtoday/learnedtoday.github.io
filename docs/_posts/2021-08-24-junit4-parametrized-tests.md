---
layout: post
title: JUnit4 Parametrized tests
date: 2021-08-24 16:46 +0200
---

The custom runner Parameterized implements parameterized tests. When running a parameterized test class, instances are created for the cross-product of the test methods and the test data elements.

For example:

```
@RunWith(Parameterized::class)
class EmailValidatorTest(
    private val input: String,
    private val expected:Boolean
) {

    @Test
    fun test() {
        assertThat(EmailValidator.validate(input)).isEqualTo(expected)
    }

    companion object {
        @JvmStatic
        @Parameterized.Parameters
        fun data() = arrayOf(
            arrayOf("test@kotl.in", true),
            arrayOf("test @kotl .in", false)
        )
    }
}
```
