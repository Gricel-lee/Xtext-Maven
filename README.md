# Xtext-Maven
Error when integrating an standalone of my Xtext project into Maven.


```
Hi
Exception in thread "main" com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.FactoryProxy.notify(FactoryProxy.java:46)
	at com.google.inject.internal.ProcessedBindingData.runCreationListeners(ProcessedBindingData.java:50)
	at com.google.inject.internal.InternalInjectorCreator.initializeStatically(InternalInjectorCreator.java:133)
	at com.google.inject.internal.InternalInjectorCreator.build(InternalInjectorCreator.java:106)
	at com.google.inject.Guice.createInjector(Guice.java:95)
	at com.google.inject.Guice.createInjector(Guice.java:72)
	at com.google.inject.Guice.createInjector(Guice.java:62)
	at org.eclipse.xtext.common.TerminalsStandaloneSetupGenerated.createInjector(TerminalsStandaloneSetupGenerated.java:40)
	at org.eclipse.xtext.common.TerminalsStandaloneSetupGenerated.createInjectorAndDoEMFRegistration(TerminalsStandaloneSetupGenerated.java:34)
	at org.eclipse.xtext.common.TerminalsStandaloneSetup.doSetup(TerminalsStandaloneSetup.java:11)
	at zzz.example.mydsl1.MyDslStandaloneSetupGenerated.createInjectorAndDoEMFRegistration(MyDslStandaloneSetupGenerated.java:21)
	at run.main(run.java:19)
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.MembersInjectorStore.get(MembersInjectorStore.java:65)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:73)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 23 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.createImplementedByBinding(InjectorImpl.java:732)
	at com.google.inject.internal.InjectorImpl.createUninitializedBinding(InjectorImpl.java:618)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:845)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.SingleFieldInjector.<init>(SingleFieldInjector.java:41)
	at com.google.inject.internal.MembersInjectorStore.getInjectors(MembersInjectorStore.java:125)
	at com.google.inject.internal.MembersInjectorStore.createWithListeners(MembersInjectorStore.java:95)
	at com.google.inject.internal.MembersInjectorStore.access$000(MembersInjectorStore.java:34)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:42)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:39)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 33 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.MembersInjectorStore.get(MembersInjectorStore.java:65)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:73)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 58 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.createImplementedByBinding(InjectorImpl.java:732)
	at com.google.inject.internal.InjectorImpl.createUninitializedBinding(InjectorImpl.java:618)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:845)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.SingleFieldInjector.<init>(SingleFieldInjector.java:41)
	at com.google.inject.internal.MembersInjectorStore.getInjectors(MembersInjectorStore.java:125)
	at com.google.inject.internal.MembersInjectorStore.createWithListeners(MembersInjectorStore.java:95)
	at com.google.inject.internal.MembersInjectorStore.access$000(MembersInjectorStore.java:34)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:42)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:39)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 68 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.MembersInjectorStore.get(MembersInjectorStore.java:65)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:73)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 93 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.createImplementedByBinding(InjectorImpl.java:732)
	at com.google.inject.internal.InjectorImpl.createUninitializedBinding(InjectorImpl.java:618)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:845)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.SingleFieldInjector.<init>(SingleFieldInjector.java:41)
	at com.google.inject.internal.MembersInjectorStore.getInjectors(MembersInjectorStore.java:125)
	at com.google.inject.internal.MembersInjectorStore.createWithListeners(MembersInjectorStore.java:95)
	at com.google.inject.internal.MembersInjectorStore.access$000(MembersInjectorStore.java:34)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:42)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:39)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 103 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.MembersInjectorStore.get(MembersInjectorStore.java:65)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:73)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 128 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.createImplementedByBinding(InjectorImpl.java:732)
	at com.google.inject.internal.InjectorImpl.createUninitializedBinding(InjectorImpl.java:618)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:845)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.SingleFieldInjector.<init>(SingleFieldInjector.java:41)
	at com.google.inject.internal.MembersInjectorStore.getInjectors(MembersInjectorStore.java:125)
	at com.google.inject.internal.MembersInjectorStore.createWithListeners(MembersInjectorStore.java:95)
	at com.google.inject.internal.MembersInjectorStore.access$000(MembersInjectorStore.java:34)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:42)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:39)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 138 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.MembersInjectorStore.get(MembersInjectorStore.java:65)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:73)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 163 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.createImplementedByBinding(InjectorImpl.java:732)
	at com.google.inject.internal.InjectorImpl.createUninitializedBinding(InjectorImpl.java:618)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:845)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.SingleFieldInjector.<init>(SingleFieldInjector.java:41)
	at com.google.inject.internal.MembersInjectorStore.getInjectors(MembersInjectorStore.java:125)
	at com.google.inject.internal.MembersInjectorStore.createWithListeners(MembersInjectorStore.java:95)
	at com.google.inject.internal.MembersInjectorStore.access$000(MembersInjectorStore.java:34)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:42)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:39)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 173 more
Caused by: com.google.inject.internal.util.$ComputationException: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.MembersInjectorStore.get(MembersInjectorStore.java:65)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:73)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 198 more
Caused by: com.google.inject.internal.util.$ComputationException: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:553)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:419)
	at com.google.inject.internal.util.$CustomConcurrentHashMap$ComputingImpl.get(CustomConcurrentHashMap.java:2041)
	at com.google.inject.internal.FailableCache.get(FailableCache.java:50)
	at com.google.inject.internal.ConstructorInjectorStore.get(ConstructorInjectorStore.java:49)
	at com.google.inject.internal.ConstructorBindingImpl.initialize(ConstructorBindingImpl.java:125)
	at com.google.inject.internal.InjectorImpl.initializeJitBinding(InjectorImpl.java:521)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBinding(InjectorImpl.java:847)
	at com.google.inject.internal.InjectorImpl.createJustInTimeBindingRecursive(InjectorImpl.java:772)
	at com.google.inject.internal.InjectorImpl.getJustInTimeBinding(InjectorImpl.java:256)
	at com.google.inject.internal.InjectorImpl.getBindingOrThrow(InjectorImpl.java:205)
	at com.google.inject.internal.InjectorImpl.getInternalFactory(InjectorImpl.java:853)
	at com.google.inject.internal.SingleFieldInjector.<init>(SingleFieldInjector.java:41)
	at com.google.inject.internal.MembersInjectorStore.getInjectors(MembersInjectorStore.java:125)
	at com.google.inject.internal.MembersInjectorStore.createWithListeners(MembersInjectorStore.java:95)
	at com.google.inject.internal.MembersInjectorStore.access$000(MembersInjectorStore.java:34)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:42)
	at com.google.inject.internal.MembersInjectorStore$1.create(MembersInjectorStore.java:39)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 208 more
Caused by: java.lang.ExceptionInInitializerError
	at com.google.inject.internal.cglib.reflect.$FastClassEmitter.<init>(FastClassEmitter.java:67)
	at com.google.inject.internal.cglib.reflect.$FastClass$Generator.generateClass(FastClass.java:72)
	at com.google.inject.internal.cglib.core.$DefaultGeneratorStrategy.generate(DefaultGeneratorStrategy.java:25)
	at com.google.inject.internal.cglib.core.$AbstractClassGenerator.create(AbstractClassGenerator.java:216)
	at com.google.inject.internal.cglib.reflect.$FastClass$Generator.create(FastClass.java:64)
	at com.google.inject.internal.BytecodeGen.newFastClass(BytecodeGen.java:207)
	at com.google.inject.internal.DefaultConstructionProxyFactory.create(DefaultConstructionProxyFactory.java:53)
	at com.google.inject.internal.ProxyFactory.create(ProxyFactory.java:153)
	at com.google.inject.internal.ConstructorInjectorStore.createConstructor(ConstructorInjectorStore.java:89)
	at com.google.inject.internal.ConstructorInjectorStore.access$000(ConstructorInjectorStore.java:28)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:36)
	at com.google.inject.internal.ConstructorInjectorStore$1.create(ConstructorInjectorStore.java:32)
	at com.google.inject.internal.FailableCache$1.apply(FailableCache.java:39)
	at com.google.inject.internal.util.$MapMaker$StrategyImpl.compute(MapMaker.java:549)
	... 227 more
Caused by: java.lang.reflect.InaccessibleObjectException: Unable to make protected final java.lang.Class java.lang.ClassLoader.defineClass(java.lang.String,byte[],int,int,java.security.ProtectionDomain) throws java.lang.ClassFormatError accessible: module java.base does not "opens java.lang" to unnamed module @7dc19a70
	at java.base/java.lang.reflect.AccessibleObject.checkCanSetAccessible(AccessibleObject.java:354)
	at java.base/java.lang.reflect.AccessibleObject.checkCanSetAccessible(AccessibleObject.java:297)
	at java.base/java.lang.reflect.Method.checkCanSetAccessible(Method.java:199)
	at java.base/java.lang.reflect.Method.setAccessible(Method.java:193)
	at com.google.inject.internal.cglib.core.$ReflectUtils$2.run(ReflectUtils.java:56)
	at java.base/java.security.AccessController.doPrivileged(AccessController.java:318)
	at com.google.inject.internal.cglib.core.$ReflectUtils.<clinit>(ReflectUtils.java:46)
	... 241 more

```
