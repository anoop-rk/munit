## Munit Processors
> https://docs.mulesoft.com/munit/2.3/event-processors
### Assert Expression
- The Assert Expression processor allows you evaluate a Dataweave expression that asserts the state of a Mule Event’s content. 
- It uses dataweave assertions library 
- The DW assertions library allows you to assert the state of the Mule Event’s content in a deeper way.
> https://docs.mulesoft.com/munit/2.3/assertion-expression-processor

> https://docs.mulesoft.com/munit/2.3/dataweave-assertions-library

### Assert That
- The Assert That processor uses a set of DataWeave functions called MUnit matchers to define the assertion conditions for any value in an expression.
> https://docs.mulesoft.com/munit/2.3/assertion-event-processor

> https://docs.mulesoft.com/munit/2.3/munit-matchers

### Assert Equals
- to assert that a payload is equal to a certain value, you can configure the Assert-Equals processor the following way

```xml
<munit-tools:assert-equals
  actual="#[payload]"
  expected="Example"
  message="The payload should be 'Example'"/>
```
- If this assertion fails, the processor throws a `java.lang.AssertionError`.
> https://docs.mulesoft.com/munit/2.3/assertion-equals-processor

### Storage Event Processors
- The Storage processors allows you to manage temporary storage during your tests.

- All storage is cleared as soon as the test ends.

1. Store
2. Retrive
3. Remove
4. Clear Stored Data

> https://docs.mulesoft.com/munit/2.3/storage-event-processors

### Queue Event Processors
1. Queue
2. Dequeue
3. Queue Size
> https://docs.mulesoft.com/munit/2.3/queue-processors

### Run Custom Event Processor
- The Run Custom event processor allows you to assert the Mule event content against a custom assertion.
> https://docs.mulesoft.com/munit/2.3/run-custom-event-processor

### Sleep Processor
- The Sleep processor allows you to pause your test for a specific time. You can use this processor to simulate a delay in the processing of the flow
> https://docs.mulesoft.com/munit/2.3/sleep-processor