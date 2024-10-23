## def

on définit notre service en tant que provider au sein de

- l’application avec bootsrap/provindInRoot
- du module avec @Ngmodule providers
- dans un composant avec @Component providers

La dependency injection = singleton + lazy loading

## Utilisation

- délcaration dans le contructeur :
    - constructor(private backend: BackendService) {}
- avec Injector :
    - private backend = inject(BackendService);

## dependency provider

- The `provide` property holds the token that serves as the key for consuming the dependency value.
- The second property is a provider definition object, which tells the injector **how** to create the dependency value. The provider-definition can be one of the following:
    - `useClass` - this option tells Angular DI to instantiate a provided class when a dependency is injected
    - `useExisting` - allows you to alias a token and reference any existing one.
    - `useFactory` - allows you to define a function that constructs a dependency.
    - `useValue` - provides a static value that should be used as a dependency.

pas tout compris à revoir