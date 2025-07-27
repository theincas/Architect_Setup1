Core

├── Application

│   ├── DTOs

│   ├── Commands

│   ├── Queries

│   └── Interfaces

├── Domain

│   ├── Entities

│   ├── ValueObjects

│   └── Enums


Infrastructure

├── Persistence

│   └── EfRepositories

UI
├── WebUI

│   └── Controllers


This is a draft of my own architecture. It basically provides a clear architecture based on SOLID principles.


[ UI Layer ] ---------------------------┐

    (WebUI, Controllers)               |
    
                ↓                     |
                
[ Application Layer ] <-------------┐ |

    (UseCases, DTOs, Interfaces)    | |
    
                ↓                  | |
                
[ Domain Layer ]                   | |

    (Entities, ValueObjects)       | |
    
                                   | |
                                   
[ Infrastructure Layer ] ----------┘ |

    (Persistence, EfRepositories,   |
    
