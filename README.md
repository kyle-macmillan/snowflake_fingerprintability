### Evaluating Snowflake as an Indistinguishable Censorship Circumvention Tool
Tor is the most well-known tool for circumventing censorship.Unfortunately, Tor traffic has been shown to be detectable us-ing deep-packet inspection. WebRTC is a popular web frame-work that enables browser-to-browser connections. Snowflake is a novel pluggable transport that leverages WebRTC to connect Tor clients to the Tor network. In theory, Snowflake was created to be indistinguishable from other WebRTC services. In this  paper,  we  evaluate  the  indistinguishability  of Snowflake. We collect over 5,500 DTLS handshakes from Snowflake, Facebook Messenger, Google Hangouts, and Discord WebRTC connections and show that Snowflake is identifiable among these applications with 100% accuracy. We show that several features, including the extensions offered and the number of packets in the handshake, distinguish Snowflake among these WebRTC-based services. Finally, we suggest recommendations for improving identification resistance in Snowflake.



### Dataset
We collect data by capturing isolated DTLS handshakes from WebRTC connections. The following table summarizes the handshakes collected.
|         | Snowflake | Facebook Messenger | Google Hangouts | Discord |
|---------|-----------|--------------------|-----------------|---------|
| Firefox | 991       | 796                | 756             | 992     |
| Chrome  | 0         | 784                | 471             | 997     |
| Total   | 991       | 1580               | 1227            | 1989    |
