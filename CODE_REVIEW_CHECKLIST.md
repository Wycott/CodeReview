# Code Review Checklist

## About

This checklist hopes to provide a basic quality gate that can be applied to most code reviews.

Once you've reviewed the same code a number of times, it can be tempting just to check for a few basic issues and waive code through, but it is incumbent on the reviewer to catch all issues as early as possible.

## Limitations

While I would hope there is some value here for any language, it is primarily designed with OO languages in mind.

N.B. modern code quality tools now take care of some of these, but the general principles still stand.

## Advisory

I would suggest that all code is reviewed with the same rigour whether it purports to be throw away code or changes to production code.

> Todays quick fix is tomorrows technical debt.

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

**To keep things simple, I’ve marked only one category per check, even though several could apply in practice.**

---

*Created: 19 December 2025*  
*Updated: 19 December 2025*