# Code Review Checklist

## About

For various reasons, basic standards around code reviews haven't always been in place in the various places I've worked.

So this document aims to change that and I've taken it from place to place since I started it circa 2010.

As well as being freely available to any of my colleagues, it is also there to keep me honest when I am short on time.

It is all to easy to waive through some code when you've seen it for about the tenth time. But experience tells me that even minor issues can get left under the pressure of delivery.

## Limitations

While I would hope there is value here for any language it is primarily designed with OO languages in mind.

Some of the items in the checklist are taken care of by various quality tools but I've resisted the urge to remove these as the principals still stand. And also, these may not be available for all languages.

## Checklist

| Check                                                                    | Category     | Pass/Fail |
|--------------------------------------------------------------------------|--------------|-----------|
| Does the code solve the problem                                          | Requirements | ✅ / ❌  |
| Are class and variable names meaningful                                  | Readability  | ✅ / ❌  |
| Is the code readable and maintainable                                    | Readability  | ✅ / ❌  |
| Could the code be more efficient                                         | Cruft        | ✅ / ❌  |
| Are there orphan/empty methods that could be removed                     | Cruft        | ✅ / ❌  |
| Does the code compile without warnings                                   | Code Quality | ✅ / ❌  |
| Have ReSharper or other code quality tool warnings been dealt with       | Code Quality | ✅ / ❌  |
| Is the code free of magic numbers or literals                            | Code Quality | ✅ / ❌  |
| Are parameters correctly validated                                       | Code Quality | ✅ / ❌  |
| Does the code follow SOLID principles                                    | Code Quality | ✅ / ❌  |
| Does the code follow DRY principles                                      | Code Quality | ✅ / ❌  |
| Is the code style consistent                                             | Code Quality | ✅ / ❌  |
| Are exceptions handled gracefully                                        | Code Quality | ✅ / ❌  |
| Are unit tests present                                                   | Testing      | ✅ / ❌  |
| Do the unit tests pass                                                   | Testing      | ✅ / ❌  |
| Is there any new code not covered by a unit test                         | Testing      | ✅ / ❌  |
| Can the code be run                                                      | Testing      | ✅ / ❌  |
| Have TODOs been dealt                                                    | Comments     | ✅ / ❌  |
| Has commented out code been removed                                      | Comments     | ✅ / ❌  |
| Are there comments that simply describe clear code                       | Comments     | ✅ / ❌  |
| Are there comments that describe complex code that should be refactored  | Comments     | ✅ / ❌  |
| Are there comments that will require maintenance for simple code changes | Comments     | ✅ / ❌  |

---

*Created: 19 December 2025*  
*Updated: 19 December 2025*