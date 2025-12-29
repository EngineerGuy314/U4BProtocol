<div class="WordSection1">

# <span id="__RefHeading___Toc2111_1057631513"></span>U4BProtocol Specification

# <span style="font-size:20.0pt">w/references to WsprEncoded C/Python Libraries </span>

Current versions

U4BProtocol Specification v1.1

WsprEncoded Library v4.3.2

Table of Contents

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">U4BProtocol &WsprEncoded C/Python Libraries Specification.............................................................. 1</span></span>](#__RefHeading___Toc2111_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Intent.......................................................................................................................................................... 4</span></span>](#__RefHeading___Toc2113_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Updates...................................................................................................................................................... 5</span></span>](#__RefHeading___Toc2115_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">History....................................................................................................................................................... 5</span></span>](#__RefHeading___Toc2117_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">License....................................................................................................................................................... 5</span></span>](#__RefHeading___Toc2119_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Basic Telemetry......................................................................................................................................... 6</span></span>](#__RefHeading___Toc2121_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Overview............................................................................................................................................... 6</span></span>](#__RefHeading___Toc2123_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Message Format.................................................................................................................................... 6</span></span>](#__RefHeading___Toc2125_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Telemetry Fields.................................................................................................................................... 7</span></span>](#__RefHeading___Toc2127_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Field Specifications.......................................................................................................................... 7</span></span>](#__RefHeading___Toc2129_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Grid Position Enhancement (Grid5 & Grid6).................................................................................. 7</span></span>](#__RefHeading___Toc2131_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Purpose........................................................................................................................................ 7</span></span>](#__RefHeading___Toc2133_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Resolution Improvement............................................................................................................. 7</span></span>](#__RefHeading___Toc2135_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding...................................................................................................................................... 7</span></span>](#__RefHeading___Toc2137_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Example....................................................................................................................................... 7</span></span>](#__RefHeading___Toc2139_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Altitude Measurement...................................................................................................................... 7</span></span>](#__RefHeading___Toc2141_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Specification................................................................................................................................ 7</span></span>](#__RefHeading___Toc2143_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Usage........................................................................................................................................... 8</span></span>](#__RefHeading___Toc2145_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Temperature Measurement............................................................................................................... 8</span></span>](#__RefHeading___Toc2147_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Specification................................................................................................................................ 8</span></span>](#__RefHeading___Toc2149_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Rollover Behavior....................................................................................................................... 8</span></span>](#__RefHeading___Toc2151_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Rollover Example........................................................................................................................ 8</span></span>](#__RefHeading___Toc2153_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Voltage Measurement....................................................................................................................... 8</span></span>](#__RefHeading___Toc2155_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Specification................................................................................................................................ 8</span></span>](#__RefHeading___Toc2157_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Standard Rollover Ranges........................................................................................................... 9</span></span>](#__RefHeading___Toc2159_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding...................................................................................................................................... 9</span></span>](#__RefHeading___Toc2161_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Alternative Encoding example for only 3.0 to 4.95v with clamping.......................................... 9</span></span>](#__RefHeading___Toc2163_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Decoding voltage assuming it represents 3.0 to 4.95v range at original measurement.............. 9</span></span>](#__RefHeading___Toc2165_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Speed Measurement......................................................................................................................... 9</span></span>](#__RefHeading___Toc2167_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Specification................................................................................................................................ 9</span></span>](#__RefHeading___Toc2169_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Usage......................................................................................................................................... 10</span></span>](#__RefHeading___Toc2171_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">GPS Validity Flag........................................................................................................................... 10</span></span>](#__RefHeading___Toc2173_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Purpose...................................................................................................................................... 10</span></span>](#__RefHeading___Toc2175_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Values........................................................................................................................................ 10</span></span>](#__RefHeading___Toc2177_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Usage......................................................................................................................................... 10</span></span>](#__RefHeading___Toc2179_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Telemetry Type Header.................................................................................................................. 10</span></span>](#__RefHeading___Toc2181_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Purpose...................................................................................................................................... 10</span></span>](#__RefHeading___Toc2183_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Values........................................................................................................................................ 10</span></span>](#__RefHeading___Toc2185_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Usage......................................................................................................................................... 10</span></span>](#__RefHeading___Toc2187_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding examples............................................................................................................................. 10</span></span>](#__RefHeading___Toc2189_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">encodeBasicTelemetry()............................................................................................................ 10</span></span>](#__RefHeading___Toc2191_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">decodeBasicTelemetry()............................................................................................................ 11</span></span>](#__RefHeading___Toc2193_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Complete Example......................................................................................................................... 11</span></span>](#__RefHeading___Toc2195_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding Architecture........................................................................................................................ 12</span></span>](#__RefHeading___Toc2197_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Two-Stage Encoding Process......................................................................................................... 12</span></span>](#__RefHeading___Toc2199_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Stage 1: Callsign Encoding....................................................................................................... 12</span></span>](#__RefHeading___Toc2201_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Stage 2: Grid+Power Encoding................................................................................................. 12</span></span>](#__RefHeading___Toc2203_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Rollover Considerations................................................................................................................. 12</span></span>](#__RefHeading___Toc2205_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Advantages................................................................................................................................ 12</span></span>](#__RefHeading___Toc2207_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Disadvantages............................................................................................................................ 12</span></span>](#__RefHeading___Toc2209_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Best Practices............................................................................................................................. 12</span></span>](#__RefHeading___Toc2211_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Implementation-Specific Behavior..................................................................................................... 13</span></span>](#__RefHeading___Toc2213_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Example:.................................................................................................................................... 13</span></span>](#__RefHeading___Toc2215_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Voltage Range Restriction......................................................................................................... 13</span></span>](#__RefHeading___Toc2217_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Behavior Differences................................................................................................................. 13</span></span>](#__RefHeading___Toc2219_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Transmission Scheduling.................................................................................................................... 13</span></span>](#__RefHeading___Toc2221_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Selection........................................................................................................................... 13</span></span>](#__RefHeading___Toc2223_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Integration with Channel Map....................................................................................................... 14</span></span>](#__RefHeading___Toc2225_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Error Handling.................................................................................................................................... 14</span></span>](#__RefHeading___Toc2227_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Validation Functions....................................................................................................................... 14</span></span>](#__RefHeading___Toc2229_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Error Codes.................................................................................................................................... 14</span></span>](#__RefHeading___Toc2231_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Performance Characteristics............................................................................................................... 15</span></span>](#__RefHeading___Toc2233_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding Efficiency....................................................................................................................... 15</span></span>](#__RefHeading___Toc2235_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Precision Trade-offs....................................................................................................................... 15</span></span>](#__RefHeading___Toc2237_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">ChannelMap Specification....................................................................................................................... 15</span></span>](#__RefHeading___Toc2239_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Overview............................................................................................................................................. 15</span></span>](#__RefHeading___Toc2241_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Core Concepts..................................................................................................................................... 15</span></span>](#__RefHeading___Toc2243_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Message Types............................................................................................................................... 15</span></span>](#__RefHeading___Toc2245_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Identification.................................................................................................................... 15</span></span>](#__RefHeading___Toc2247_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Data Structures.................................................................................................................................... 15</span></span>](#__RefHeading___Toc2249_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Object............................................................................................................................... 15</span></span>](#__RefHeading___Toc2251_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Telemetry Message Structure......................................................................................................... 16</span></span>](#__RefHeading___Toc2253_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Identification Methods........................................................................................................................ 16</span></span>](#__RefHeading___Toc2255_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">1. ID13 Encoding........................................................................................................................... 16</span></span>](#__RefHeading___Toc2257_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Example..................................................................................................................................... 16</span></span>](#__RefHeading___Toc2259_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">2. Time Slot Identification.............................................................................................................. 16</span></span>](#__RefHeading___Toc2261_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">3. Frequency Matching................................................................................................................... 16</span></span>](#__RefHeading___Toc2263_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Target Frequency....................................................................................................................... 16</span></span>](#__RefHeading___Toc2265_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Frequency Fingerprinting, Frequency binning or other mechanisms........................................ 16</span></span>](#__RefHeading___Toc2267_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Implementation Notes......................................................................................................................... 17</span></span>](#__RefHeading___Toc2269_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Receiver Calibration Challenges.................................................................................................... 17</span></span>](#__RefHeading___Toc2271_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Fingerprinting Algorithm............................................................................................................... 17</span></span>](#__RefHeading___Toc2273_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Performance Considerations.......................................................................................................... 17</span></span>](#__RefHeading___Toc2275_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Map Integration.................................................................................................................... 17</span></span>](#__RefHeading___Toc2277_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Extended Telemetry Specification........................................................................................................... 18</span></span>](#__RefHeading___Toc2279_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Overview............................................................................................................................................. 18</span></span>](#__RefHeading___Toc2281_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Key Features................................................................................................................................... 18</span></span>](#__RefHeading___Toc2283_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Message Architecture.......................................................................................................................... 18</span></span>](#__RefHeading___Toc2285_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Message Structure.......................................................................................................................... 18</span></span>](#__RefHeading___Toc2287_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Header Fields.................................................................................................................................. 18</span></span>](#__RefHeading___Toc2289_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Header Field Details.................................................................................................................. 18</span></span>](#__RefHeading___Toc2291_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Message Types.................................................................................................................................... 19</span></span>](#__RefHeading___Toc2293_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Planned Enumerated Types (Examples)......................................................................................... 19</span></span>](#__RefHeading___Toc2295_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Time Slot Management....................................................................................................................... 19</span></span>](#__RefHeading___Toc2297_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">10-Minute Window Structure......................................................................................................... 19</span></span>](#__RefHeading___Toc2299_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Transmission Patterns..................................................................................................................... 19</span></span>](#__RefHeading___Toc2301_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Backward Compatible............................................................................................................... 19</span></span>](#__RefHeading___Toc2303_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Extended Only........................................................................................................................... 20</span></span>](#__RefHeading___Toc2305_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Mixed Mode.............................................................................................................................. 20</span></span>](#__RefHeading___Toc2307_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding Specification....................................................................................................................... 20</span></span>](#__RefHeading___Toc2309_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Data Encoding................................................................................................................................ 20</span></span>](#__RefHeading___Toc2311_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Packing Order................................................................................................................................. 20</span></span>](#__RefHeading___Toc2313_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Value Processing............................................................................................................................ 20</span></span>](#__RefHeading___Toc2315_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Example Implementation.................................................................................................................... 20</span></span>](#__RefHeading___Toc2317_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">GPS Stats Message (Hypothetical)................................................................................................ 20</span></span>](#__RefHeading___Toc2319_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Packing Example............................................................................................................................ 21</span></span>](#__RefHeading___Toc2321_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Integration Guidelines......................................................................................................................... 21</span></span>](#__RefHeading___Toc2323_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Receiver Implementation............................................................................................................... 21</span></span>](#__RefHeading___Toc2325_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Sender Implementation.................................................................................................................. 21</span></span>](#__RefHeading___Toc2327_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Fingerprinting Logic...................................................................................................................... 21</span></span>](#__RefHeading___Toc2329_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Error Handling.................................................................................................................................... 21</span></span>](#__RefHeading___Toc2331_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Invalid Messages............................................................................................................................ 21</span></span>](#__RefHeading___Toc2333_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Backward Compatibility................................................................................................................ 22</span></span>](#__RefHeading___Toc2335_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Future Extensions................................................................................................................................ 22</span></span>](#__RefHeading___Toc2337_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">WsprEncoded C++ Library...................................................................................................................... 22</span></span>](#__RefHeading___Toc2339_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Overview............................................................................................................................................. 22</span></span>](#__RefHeading___Toc2341_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Features............................................................................................................................................... 22</span></span>](#__RefHeading___Toc2343_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Core Capabilities............................................................................................................................ 22</span></span>](#__RefHeading___Toc2345_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Design Principles............................................................................................................................ 22</span></span>](#__RefHeading___Toc2347_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Installation........................................................................................................................................... 23</span></span>](#__RefHeading___Toc2349_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Arduino Library Manager.............................................................................................................. 23</span></span>](#__RefHeading___Toc2351_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">CMake Integration.......................................................................................................................... 23</span></span>](#__RefHeading___Toc2353_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Option 1: FetchContent (Recommended).................................................................................. 23</span></span>](#__RefHeading___Toc2355_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Option 2: Git Submodules......................................................................................................... 23</span></span>](#__RefHeading___Toc2357_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Option 3: External Directory..................................................................................................... 23</span></span>](#__RefHeading___Toc2359_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">API Reference..................................................................................................................................... 23</span></span>](#__RefHeading___Toc2361_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Core Headers.................................................................................................................................. 23</span></span>](#__RefHeading___Toc2363_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Basic Telemetry API....................................................................................................................... 23</span></span>](#__RefHeading___Toc2365_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Common Measurement Types................................................................................................... 23</span></span>](#__RefHeading___Toc2367_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Encoding Functions................................................................................................................... 24</span></span>](#__RefHeading___Toc2369_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Usage Example.......................................................................................................................... 24</span></span>](#__RefHeading___Toc2371_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Extended Telemetry API................................................................................................................ 25</span></span>](#__RefHeading___Toc2373_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Custom Field Definition............................................................................................................ 25</span></span>](#__RefHeading___Toc2375_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Custom Telemetry Example...................................................................................................... 25</span></span>](#__RefHeading___Toc2377_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Map API........................................................................................................................... 26</span></span>](#__RefHeading___Toc2379_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Information.................................................................................................................. 26</span></span>](#__RefHeading___Toc2381_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Channel Map Example.............................................................................................................. 26</span></span>](#__RefHeading___Toc2383_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Complete Integration Example........................................................................................................... 27</span></span>](#__RefHeading___Toc2385_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Arduino Tracker Implementation................................................................................................... 27</span></span>](#__RefHeading___Toc2387_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Desktop Application Integration.................................................................................................... 27</span></span>](#__RefHeading___Toc2389_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Error Handling.................................................................................................................................... 28</span></span>](#__RefHeading___Toc2391_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Common Error Codes..................................................................................................................... 28</span></span>](#__RefHeading___Toc2393_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Best Practices................................................................................................................................. 28</span></span>](#__RefHeading___Toc2395_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Performance Notes.............................................................................................................................. 29</span></span>](#__RefHeading___Toc2397_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Memory Usage............................................................................................................................... 29</span></span>](#__RefHeading___Toc2399_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Processing Speed............................................................................................................................ 29</span></span>](#__RefHeading___Toc2401_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Platform Support................................................................................................................................. 29</span></span>](#__RefHeading___Toc2403_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Tested Platforms............................................................................................................................. 29</span></span>](#__RefHeading___Toc2405_1057631513)

[<span class="IndexLink"><span style="color:windowtext;text-decoration:none">Compiler Requirements................................................................................................................. 29</span></span>](#__RefHeading___Toc2407_1057631513)

 

# <span id="__RefHeading___Toc2113_1057631513"></span>Intent

QRPLabs for some time has sold a tracker <https://www.qrp-labs.com/u4b.html> that has a behavior for transmitting WSPR packets to convey information from a balloon in flight over planet Earth. This info is received by worldwide WSPR receivers, and the data uploaded to accessible databases like wsprlive and wsprnet.

A number of trackers have been produced, some open-source and available on github.com that have behavior compatible with the QRPLabs U4B “protocol”. Additionally, websites have been created, or other software, that interprets the WSPR data and creates various analysis or visualizations.

The behavior of this protocol has changed over time, and various software may or may not support what is considered the “current definition”. That is fine. There is a discussion process at <https://groups.io/g/picoballoon> that attempts to keep all interested parties in alignment over time, with the benefit of shared software or website use, and to avoid conflict..i.e. one person’s tracker garbling correct reception of information from another person’s tracker.

QRPLabs has graciously allowed this compatible reverse-engineering. Hans G0UPL, over time, has released details of the U4B behaviors, which can be considered “U4B Protocol”.

 QRPLabs is under no agreement to comply in the future with anything here, and this spec does not cover all behaviors of a QRPLabs U4B tracker.

The goal is to serve a common interest for all people in the u4b or u4b-compatible world, and create more fun!

Part of the fun is innovation. Change over time should be slow to minimize chaos in the U4B-compatible world,  but hopefully it continues to happen. Important changes will be highlighted in the Updates section.

Some specification detail available on [https://www.qrp-labs.com](https://www.qrp-labs.com/) may be out of date and not reflect the true current behavior of U4B trackers.

This spec should be considered the current community consensus. Issues or Discussion can be posted at

<span class="MsoHyperlink">https://github.com/traquito/WsprEncoded</span>

<https://github.com/traquito/WsprEncodedPython>  
  
The intent is easy understanding by non-English speakers. It may take some time to get to a good spec, so revisions may happen more quickly during 2025.

# <span id="__RefHeading___Toc2115_1057631513"></span>Updates

V1.1 Initial release at the current repo: [https://github.com/knormoyle/U4BProtocol](https://github.com/knormoyle/WsprEncoded)

# <span id="__RefHeading___Toc2117_1057631513"></span>History

U3B and U3S WSPR on balloons appeared around 2015, with U4B development after that by Hans G0UPL and Dave VE3KCL.

Some other trackers reverse-engineered U4B protocol, but Doug KD2KDD did extensive work in that area starting in 2023. This was called the Traquito project.

Doug KD2KDD organized a collaborative effort to extend U4B protocol in 12/24 and made the extensions (Extended Telemetry) available under AGPL.

The original U4B protocol before 12/24 is considered to be Basic Telemetry. The extensions are considered to be Extended Telemery. Hans G0UPL aligned QRPLabs U4B firmware to the Extended Telemetry spec around 7/25.

The supporting library and clarity of definition here, are all because of Doug’s work, and the community thanks him for his time and commitment to the idea.

# <span id="__RefHeading___Toc2119_1057631513"></span>License

This specification and the WsprEncoded library is under AGPL license.

This document provides specification for Basic and Extended U4B protocol, definition of channels to isolate telemetry from different transmitters, and a description of the WsprEncoded library available at** ** <https://github.com/traquito/WsprEncoded><span class="MsoHyperlink"> </span>to simplify implementation of the protocol.

Contributions, modifications and extensions are encouraged and merges will be accepted via <https://github.com/knormoyle/U4BProtocol> repo.

U4BProtocol includes Basic Telemetry and Extended Telemetry. QRPLabs has some alternative transmissions with its legacy TELE instruction that are not part of this spec. The QRPLabs TELEX command meets the Extended Telemetry spec.

# <span id="__RefHeading___Toc2121_1057631513"></span>Basic Telemetry

## <span id="__RefHeading___Toc2123_1057631513"></span>Overview

The Basic Telemetry API provides a standardized method for encoding common tracker measurements into WSPR Type 1 messages. This system enables transmission of GPS location, environmental sensors, and system status information through the WSPR protocol's 50-bit data capacity. 

<span style="color:#333333">Note that there can be bad GPS data on altitude, latitude and longitude, and voltage measurement can be bad also.</span>

<span style="color:#333333">For example, if the tracker is not getting 3.3v to an rp2040 and rp2040 voltage measurement is only "right" if supply voltage to the rp2040 and the temperature ADC is getting a correct 3.3v compare voltage. A tracker may implement additional filtering or clamping to deal with those issues. </span>

<span style="color:#333333">The language below governs what result happens on a website if no such filtering happens, i.e. what values are reported from particular encoded values.</span>

<span style="color:#333333">Note there is no such thing as Nan or Invalid encodings. So it’s important to understand that Basic Telemetry will always decode to something. You always get an answer. The validity of that answer depends on an understanding of all of U4B Protocol.</span>

<span style="color:#333333">Decoding of random unused callsign space spots from wsprlive will show that everything can decode to something (even it's out of the valid range of the intermediate "big number" for U4B protocol, if there is no checking for that).</span>

<span style="color:#333333">The current basic telemetry doesn't fully occupy the space allowed by the wspr big-number encoding process. So just being able to decode something doesn’t validate that it’s U4B Protocol information.</span>

It’s possible that unused big number space could be used for "anything" like NaN or None. Place holder for the future.

 

A common case is accidentally decoding WB8ELK protocol telemetry. It will sometimes have a intermediate big number range that’s illegal relative to U4B protocol telemetry. A website could detect that. It can be discovered by looking at the big number being out-of-expected-range, or having a remainder left over after decoding all known U4B protocol subfields from the big number.

 

## <span id="__RefHeading___Toc2125_1057631513"></span>Message Format

Basic Telemetry messages use the WSPR Type 1 format with specific field allocations:

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\<callsign\> \<grid\> \<power\></span>

<span class="SourceText">\`\`\`</span>

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Field Mapping:</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Callsign</span>**: Encodes Grid5, Grid6, and Altitude

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Grid</span>**: Encodes Temperature, Voltage, Speed, GPS validity, and telemetry type

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Power</span>**: Part of the encoding scheme

## <span id="__RefHeading___Toc2127_1057631513"></span>Telemetry Fields

### <span id="__RefHeading___Toc2129_1057631513"></span>Field Specifications

| Field Name       | Unit      | Min Value | Max Value | Step Size | Possible Values |
|------------------|-----------|-----------|-----------|-----------|-----------------|
| Grid5            | Character | 0         | 23        | 1         | 24              |
| Grid6            | Character | 0         | 23        | 1         | 24              |
| Altitude         | Meters    | 0         | 21,340    | 20        | 1,068           |
| Temperature      | Celsius   | -50       | 39        | 1         | 90              |
| Voltage          | Volts     | 2.0       | 3.95      | 0.05      | 40              |
| Speed            | Knots     | 0         | 82        | 2         | 42              |
| IsGpsValid       | Boolean   | 0         | 1         | 1         | 2               |
| HdrTelemetryType | Enum      | 0         | 1         | 1         | 2               |

###  

### <span id="__RefHeading___Toc2131_1057631513"></span>Grid Position Enhancement (Grid5 & Grid6)

#### <span id="__RefHeading___Toc2133_1057631513"></span>Purpose

Extends the 4-character WSPR grid to 6 characters for improved location precision.

#### <span id="__RefHeading___Toc2135_1057631513"></span>Resolution Improvement

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">4-character grid</span>**: 70 × 140 miles resolution

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">6-character grid</span>**: 3 × 3 miles resolution

#### <span id="__RefHeading___Toc2137_1057631513"></span>Encoding

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Grid5 and Grid6 encode characters A-X (values 0-23)</span>

<span class="SourceText">char grid5_char = 'A' + grid5_value;  // grid5_value: 0-23</span>

<span class="SourceText">char grid6_char = 'A' + grid6_value;  // grid6_value: 0-23</span>

<span class="SourceText"> </span>

<span class="SourceText">// Complete 6-character grid formation</span>

<span class="SourceText">std::string full_grid = wspr_grid_4char + grid5_char + grid6_char;</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2139_1057631513"></span>Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// WSPR Type 1 grid: "FN31"</span>

<span class="SourceText">// Grid5 = 12 (M), Grid6 = 7 (H)</span>

<span class="SourceText">// Complete grid: "FN31MH"</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2141_1057631513"></span>Altitude Measurement

#### <span id="__RefHeading___Toc2143_1057631513"></span>Specification

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Source</span>**: GPS-derived elevation

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Range</span>**: 0 to 21,340 meters

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Resolution</span>**: 20-meter steps

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Encoding</span>**: Linear quantization with rollover support

#### <span id="__RefHeading___Toc2145_1057631513"></span>Usage

<span class="SourceText">\`\`\`</span>

<span class="SourceText">uint16_t encodeAltitude(uint16_t altitude_meters) {</span>

<span class="SourceText">    // Rollover at 21340m. </span>

<span class="SourceText">    // Trackers may optionally clamp to min/max range</span>

<span class="SourceText">    // Negative numbers should also be filtered, in case of bad gps data</span>

<span class="SourceText">    altitude_meters = altitude_meters % 21340;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Quantize to 20m steps</span>

<span class="SourceText">    return altitude_meters / 20;</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">uint16_t decodeAltitude(uint16_t encoded_value) {</span>

<span class="SourceText">    return encoded_value \* 20;  // Convert back to meters</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2147_1057631513"></span>Temperature Measurement

#### <span id="__RefHeading___Toc2149_1057631513"></span>Specification

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Source</span>**: Environmental sensor or onboard temperature sensor

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Range</span>**: -50°C to +39°C

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Resolution</span>**: 1°C steps

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Encoding</span>**: Offset binary with rollover

#### <span id="__RefHeading___Toc2151_1057631513"></span>Rollover Behavior

<span class="SourceText">\`\`\`</span>

<span class="SourceText">int16_t encodeTemperature(int16_t temp_celsius) {</span>

<span class="SourceText">    // Apply offset and rollover. </span>

<span class="SourceText">    // Trackers should filter for negative results and do something (clamp?)</span>

<span class="SourceText">    return (temp_celsius - (-50)) % 90;</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">int16_t decodeTemperature(uint16_t encoded_value) {</span>

<span class="SourceText">    // Note: Rollover means ambiguous decoding</span>

<span class="SourceText">    return encoded_value + (-50);</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2153_1057631513"></span>Rollover Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Both -45°C and +45°C encode to the same value (5)</span>

<span class="SourceText">int16_t temp1 = -45;  // encodes to: (-45 - (-50)) % 90 = 5</span>

<span class="SourceText">int16_t temp2 = 45;   // encodes to: (45 - (-50)) % 90 = 5</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2155_1057631513"></span>Voltage Measurement

#### <span id="__RefHeading___Toc2157_1057631513"></span>Specification

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Source</span>**: System input voltage monitoring

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Range</span>**: 3.0 to 4.95v is considered the standard range, although a tracker can do continual wraparound, so there is no range limits, or pick a different 1.95v range

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Resolution</span>**: 0.05V steps

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Purpose</span>**: Monitor solar panel or battery performance

#### <span id="__RefHeading___Toc2159_1057631513"></span>Standard Rollover Ranges

The voltage field can support multiple 1.95V ranges. There is no standard for how to decide what range a tracker is using though. 3.0 to 4.95v is considered the standard range. A tracker may clamp to min/max values for the range or not. Website viewers typically do not have a way of visualizing voltages correctly outside of the 3.0v to 4.95v range.

It's possible website developers could have a configurable "base voltage" so that balloons with different known voltage ranges could be supported and visualized easily. But 3-4.95v is the consensus, non-configurable range that websites should report.

Possible examples:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>2.0V to 3.95V

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>4.0V to 5.95V

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>6.0V to 7.95V

 

#### <span id="__RefHeading___Toc2161_1057631513"></span>Encoding

<span class="SourceText">\`\`\`</span>

<span class="SourceText">uint16_t encodeVoltage(float voltage) {</span>

<span class="SourceText">    uint16_t range = (uint16_t)((voltage - 2.0) / 2.0);</span>

<span class="SourceText">    float range_offset = voltage - (2.0 + range \* 2.0);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Quantize within range</span>

<span class="SourceText">    uint16_t step = (uint16_t)(range_offset / 0.05);</span>

<span class="SourceText">    </span>

<span class="SourceText">    return step % 40;  // Rollover within 40 possible values</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2163_1057631513"></span>Alternative Encoding example for only 3.0 to 4.95v with clamping

<span class="SourceText">\`\`\`</span>

<span class="SourceText">uint16_t encodeVoltage(float voltage) {</span>

<span class="SourceText">    // voltage encodings: </span>

<span class="SourceText">    // 20 to 39, 0 to 19 for 3.00 to 4.95V with a resolution of 0.05V</span>

<span class="SourceText">    // 0 to 39 encodings</span>

<span class="SourceText">    if (voltage \> 4.95) voltage = 4.95;</span>

<span class="SourceText">    else if (voltage \< 3.00) voltage = 3.00;</span>

<span class="SourceText">    // should only be 3 to 4.95</span>

<span class="SourceText">    uint16_t voltageNum = (int)(round ((voltage - 3.00) / .05) + 20) % 40;</span>

<span class="SourceText">    return voltageNum</span>

<span class="SourceText">      </span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2165_1057631513"></span>Decoding voltage assuming it represents 3.0 to 4.95v range at original measurement

<span class="SourceText">\`\`\`</span>

<span class="SourceText">uint16_t decodedVoltage(float encoded_value) {</span>

<span class="SourceText">    voltage = round((encoded_value \* 0.05) + 2.00, 2)</span>

<span class="SourceText">    return voltage</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2167_1057631513"></span>Speed Measurement

#### <span id="__RefHeading___Toc2169_1057631513"></span>Specification

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Source</span>**: GPS-derived ground speed

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Range</span>**: 0 to 82 knots

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Resolution</span>**: 2-knot steps

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Encoding</span>**: Linear quantization with rollover

#### <span id="__RefHeading___Toc2171_1057631513"></span>Usage

<span class="SourceText">\`\`\`</span>

<span class="SourceText">uint16_t encodeSpeed(uint16_t speed_knots) {</span>

<span class="SourceText">    return (speed_knots / 2) % 42;  // Rollover support</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">uint16_t decodeSpeed(uint16_t encoded_value) {</span>

<span class="SourceText">    return encoded_value \* 2;  // Convert back to knots</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2173_1057631513"></span>GPS Validity Flag

#### <span id="__RefHeading___Toc2175_1057631513"></span>Purpose

Indicates whether GPS-derived measurements (altitude, speed, grid position) are valid. Some trackers may only send callsign+telemetry when GPS is valid, so this may always be 1. QRPLabs u4b can send callsign+telemetry when GPS is not valid. Old values are used for telemetry then, although it’s possible some data should be ignored if GPS is not valid.

#### <span id="__RefHeading___Toc2177_1057631513"></span>Values

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">0 (false)</span>**: GPS lock not available, position/speed data invalid

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">1 (true)</span>**: GPS lock acquired, position/speed data valid

#### <span id="__RefHeading___Toc2179_1057631513"></span>Usage

<span class="SourceText">\`\`\`</span>

<span class="SourceText">bool gps_valid = hasGpsLock();</span>

<span class="SourceText">uint8_t gps_flag = gps_valid ? 1 : 0;</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2181_1057631513"></span>Telemetry Type Header

#### <span id="__RefHeading___Toc2183_1057631513"></span>Purpose

Identifies the telemetry format version.

#### <span id="__RefHeading___Toc2185_1057631513"></span>Values

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">0</span>**: Reserved

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">1</span>**: Standard Basic Telemetry format

#### <span id="__RefHeading___Toc2187_1057631513"></span>Usage

<span class="SourceText">\`\`\`</span>

<span class="SourceText">const uint8_t TELEMETRY_TYPE_STANDARD = 1;</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2189_1057631513"></span>Encoding examples

#### <span id="__RefHeading___Toc2191_1057631513"></span><span class="SourceText">\`\`\`</span>

#### <span class="SourceText">encodeBasicTelemetry()</span>

#### <span class="SourceText">\`\`\`</span>

Encodes all basic telemetry fields into a WSPR message.

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">\`\`\`</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">struct BasicTelemetryData {</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    uint8_t grid5;              // 0-23</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    uint8_t grid6;              // 0-23</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    uint16_t altitude_meters;   // 0-21340</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    int16_t temperature_c;      // -50 to 39</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    float voltage_v;            // 2.0-3.95 (or rollover ranges)</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    uint16_t speed_knots;       // 0-82</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    bool gps_valid;             // true/false</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    uint8_t telemetry_type;     // 1 for standard</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">};</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal"> </span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">bool encodeBasicTelemetry(</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    const BasicTelemetryData& data,</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">    WSPRMessage& message</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">);</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">decodeBasicTelemetry()</span></span>

#### <span class="SourceText"><span style="font-size:10.0pt;font-weight:normal">\`\`\`</span></span>

Decodes basic telemetry from a WSPR message.

<span class="SourceText">\`\`\`</span>

<span class="SourceText">bool decodeBasicTelemetry(</span>

<span class="SourceText">    const WSPRMessage& message,</span>

<span class="SourceText">    BasicTelemetryData& data</span>

<span class="SourceText">);</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2195_1057631513"></span>Complete Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/BasicTelemetry.h\></span>

<span class="SourceText"> </span>

<span class="SourceText">void transmitBasicTelemetry() {</span>

<span class="SourceText">    // Collect sensor data</span>

<span class="SourceText">    BasicTelemetryData telemetry = {</span>

<span class="SourceText">        .grid5 = 12,           // 'M'</span>

<span class="SourceText">        .grid6 = 7,            // 'H'</span>

<span class="SourceText">        .altitude_meters = 1200,</span>

<span class="SourceText">        .temperature_c = 25,</span>

<span class="SourceText">        .voltage_v = 3.7,</span>

<span class="SourceText">        .speed_knots = 0,</span>

<span class="SourceText">        .gps_valid = true,</span>

<span class="SourceText">        .telemetry_type = 1</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Encode to WSPR message</span>

<span class="SourceText">    WSPRMessage message;</span>

<span class="SourceText">    if (encodeBasicTelemetry(telemetry, message)) {</span>

<span class="SourceText">        // Transmit WSPR message</span>

<span class="SourceText">        printf("Transmitting: %s %s %d\n", </span>

<span class="SourceText">               message.callsign, message.grid, message.power);</span>

<span class="SourceText">        </span>

<span class="SourceText">        // Send via radio...</span>

<span class="SourceText">        transmitWSPR(message);</span>

<span class="SourceText">    }</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">void receiveBasicTelemetry(const WSPRMessage& received) {</span>

<span class="SourceText">    BasicTelemetryData telemetry;</span>

<span class="SourceText">    </span>

<span class="SourceText">    if (decodeBasicTelemetry(received, telemetry)) {</span>

<span class="SourceText">        printf("Decoded telemetry:\n");</span>

<span class="SourceText">        printf("  Location: %c%c extension\n", </span>

<span class="SourceText">               'A' + telemetry.grid5, 'A' + telemetry.grid6);</span>

<span class="SourceText">        printf("  Altitude: %d meters\n", telemetry.altitude_meters);</span>

<span class="SourceText">        printf("  Temperature: %d°C\n", telemetry.temperature_c);</span>

<span class="SourceText">        printf("  Voltage: %.2fV\n", telemetry.voltage_v);</span>

<span class="SourceText">        printf("  Speed: %d knots\n", telemetry.speed_knots);</span>

<span class="SourceText">        printf("  GPS Valid: %s\n", telemetry.gps_valid ? "Yes" : "No");</span>

<span class="SourceText">    }</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2197_1057631513"></span>Encoding Architecture

### <span id="__RefHeading___Toc2199_1057631513"></span>Two-Stage Encoding Process

Basic Telemetry uses a two-stage encoding process to fit all fields into WSPR message components:

#### <span id="__RefHeading___Toc2201_1057631513"></span>Stage 1: Callsign Encoding

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Encode Grid5, Grid6, and Altitude into callsign</span>

<span class="SourceText">BigNumber callsign_data = 0;</span>

<span class="SourceText">callsign_data = callsign_data \* 24 + grid5;</span>

<span class="SourceText">callsign_data = callsign_data \* 24 + grid6;</span>

<span class="SourceText">callsign_data = callsign_data \* 1068 + altitude_index;</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2203_1057631513"></span>Stage 2: Grid+Power Encoding

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Encode remaining fields into grid and power</span>

<span class="SourceText">BigNumber grid_power_data = 0;</span>

<span class="SourceText">grid_power_data = grid_power_data \* 90 + temperature_index;</span>

<span class="SourceText">grid_power_data = grid_power_data \* 40 + voltage_index;</span>

<span class="SourceText">grid_power_data = grid_power_data \* 42 + speed_index;</span>

<span class="SourceText">grid_power_data = grid_power_data \* 2 + gps_valid;</span>

<span class="SourceText">grid_power_data = grid_power_data \* 2 + telemetry_type;</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2205_1057631513"></span>Rollover Considerations

#### <span id="__RefHeading___Toc2207_1057631513"></span>Advantages

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Measurements not strictly limited to defined ranges

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Handles sensor readings outside nominal ranges

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Continuous operation during extreme conditions

#### <span id="__RefHeading___Toc2209_1057631513"></span>Disadvantages

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Ambiguous decoding</span>**: Multiple input values map to same encoded value

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Requires context</span>**: Additional information needed for correct interpretation

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Data loss</span>**: Precision lost due to quantization and rollover

#### <span id="__RefHeading___Toc2211_1057631513"></span>Best Practices

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Implement bounds checking before encoding</span>

<span class="SourceText">float clampVoltage(float voltage, float min_v, float max_v) {</span>

<span class="SourceText">    if (voltage \< min_v) return min_v;</span>

<span class="SourceText">    if (voltage \> max_v) return max_v;</span>

<span class="SourceText">    return voltage;</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">// Use application-specific knowledge for decoding</span>

<span class="SourceText">int16_t decodeTemperatureWithContext(uint16_t encoded, int16_t expected_range) {</span>

<span class="SourceText">    int16_t base_temp = encoded - 50;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Apply context-based correction</span>

<span class="SourceText">    while (abs(base_temp - expected_range) \> 45) {</span>

<span class="SourceText">        if (base_temp \< expected_range) {</span>

<span class="SourceText">            base_temp += 90;  // Next rollover range</span>

<span class="SourceText">        } else {</span>

<span class="SourceText">            base_temp -= 90;  // Previous rollover range</span>

<span class="SourceText">        }</span>

<span class="SourceText">    }</span>

<span class="SourceText">    </span>

<span class="SourceText">    return base_temp;</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2213_1057631513"></span>Implementation-Specific Behavior

#### <span id="__RefHeading___Toc2215_1057631513"></span>Example:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Temperature</span>**: Uses onboard RP2040 temperature sensor

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Voltage</span>**: Samples during high-load TX conditions for worst-case readings

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">GPS Validity</span>**: Always true (GPS lock required for transmission)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Rollover</span>**: Not implemented - values are clamped to ranges

#### <span id="__RefHeading___Toc2217_1057631513"></span>Voltage Range Restriction

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Traquito, for example, uses restricted voltage range</span>

<span class="SourceText">const float VOLTAGE_MIN = 3.0;</span>

<span class="SourceText">const float VOLTAGE_MAX = 4.95;</span>

<span class="SourceText"> </span>

<span class="SourceText">float clampVoltage(float voltage) {</span>

<span class="SourceText">    if (voltage \< VOLTAGE_MIN) return VOLTAGE_MIN;</span>

<span class="SourceText">    if (voltage \> VOLTAGE_MAX) return VOLTAGE_MAX;</span>

<span class="SourceText">    return voltage;</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2219_1057631513"></span>Behavior Differences

<span class="SourceText">\`\`\`</span>

<span class="SourceText">// Standard implementation with rollover</span>

<span class="SourceText">int16_t encodeTemperatureStandard(int16_t temp) {</span>

<span class="SourceText">    return (temp - (-50)) % 90;  // Rollover enabled</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">// Implementation with clamping</span>

<span class="SourceText">int16_t encodeTemperatureClamp(int16_t temp) {</span>

<span class="SourceText">    if (temp \< -50) temp = -50;   // Clamp to minimum</span>

<span class="SourceText">    if (temp \> 39) temp = 39;     // Clamp to maximum</span>

<span class="SourceText">    return temp - (-50);          // No rollover</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2221_1057631513"></span>Transmission Scheduling

### <span id="__RefHeading___Toc2223_1057631513"></span>Channel Selection

Basic Telemetry transmission timing is coordinated with the U4B ChannelMap system. The channel selection implies a starting minute for the callsign transmission. There are 5 possible starting minutes within each 10 minute interval.

<span class="SourceText">\`\`\`</span>

<span class="SourceText"> </span>

<span class="SourceText">// Check if current time slot is appropriate for Basic Telemetry</span>

<span class="SourceText">bool canTransmitBasicTelemetry(uint8_t current_minute, uint8_t channel) {</span>

<span class="SourceText">    return isBasicTelemetrySlot(current_minute, channel);</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2225_1057631513"></span>Integration with Channel Map

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/ChannelMap.h\></span>

<span class="SourceText">\#include \<WsprEncoded/BasicTelemetry.h\></span>

<span class="SourceText"> </span>

<span class="SourceText">void scheduleBasicTelemetry() {</span>

<span class="SourceText">    uint8_t current_minute = getCurrentMinute();</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Find appropriate channel for Basic Telemetry</span>

<span class="SourceText">    ChannelMap::ChannelInfo channel;</span>

<span class="SourceText">    if (ChannelMap::findBasicTelemetryChannel(20, current_minute, channel)) {</span>

<span class="SourceText">        // Encode and transmit</span>

<span class="SourceText">        BasicTelemetryData data = collectSensorData();</span>

<span class="SourceText">        WSPRMessage message;</span>

<span class="SourceText">        </span>

<span class="SourceText">        if (encodeBasicTelemetry(data, message)) {</span>

<span class="SourceText">            transmitWSPR(message, channel.frequency_hz);</span>

<span class="SourceText">        }</span>

<span class="SourceText">    }</span>

<span class="SourceText">}</span>

<span class="SourceText"> </span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2227_1057631513"></span>Error Handling

### <span id="__RefHeading___Toc2229_1057631513"></span>Validation Functions

<span class="SourceText">\`\`\`</span>

<span class="SourceText">bool validateBasicTelemetry(const BasicTelemetryData& data) {</span>

<span class="SourceText">    // Check field ranges</span>

<span class="SourceText">    if (data.grid5 \> 23 \|\| data.grid6 \> 23) return false;</span>

<span class="SourceText">    if (data.altitude_meters \> 21340) return false;</span>

<span class="SourceText">    if (data.temperature_c \< -50 \|\| data.temperature_c \> 39) return false;</span>

<span class="SourceText">    if (data.voltage_v \< 2.0 \|\| data.voltage_v \> 3.95) return false;</span>

<span class="SourceText">    if (data.speed_knots \> 82) return false;</span>

<span class="SourceText">    if (data.telemetry_type != 1) return false;</span>

<span class="SourceText">    </span>

<span class="SourceText">    return true;</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2231_1057631513"></span>Error Codes

<span class="SourceText">\`\`\`</span>

<span class="SourceText">enum class BasicTelemetryError {</span>

<span class="SourceText">    SUCCESS = 0,</span>

<span class="SourceText">    INVALID_GRID_VALUES,</span>

<span class="SourceText">    ALTITUDE_OUT_OF_RANGE,</span>

<span class="SourceText">    TEMPERATURE_OUT_OF_RANGE,</span>

<span class="SourceText">    VOLTAGE_OUT_OF_RANGE,</span>

<span class="SourceText">    SPEED_OUT_OF_RANGE,</span>

<span class="SourceText">    INVALID_TELEMETRY_TYPE,</span>

<span class="SourceText">    ENCODING_FAILED,</span>

<span class="SourceText">    DECODING_FAILED</span>

<span class="SourceText">};</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2233_1057631513"></span>Performance Characteristics

### <span id="__RefHeading___Toc2235_1057631513"></span>Encoding Efficiency

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Total fields</span>**: 8 telemetry values

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Bit utilization</span>**: ~48 of 50 available WSPR bits 

### <span id="__RefHeading___Toc2237_1057631513"></span>Precision Trade-offs

| Field       | Original Precision | Encoded Precision | Efficiency          |
|-------------|--------------------|-------------------|---------------------|
| Altitude    | 1m                 | 20m               | 95% bit utilization |
| Temperature | 0.1°C              | 1°C               | 90% bit utilization |
| Voltage     | 0.001V             | 0.05V             | 98% bit utilization |
| Speed       | 0.1 knots          | 2 knots           | 95% bit utilization |

##  

# <span id="__RefHeading___Toc2239_1057631513"></span>ChannelMap Specification

## <span id="__RefHeading___Toc2241_1057631513"></span>Overview

The ChannelMap specification enables identification and association of Telemetry messages with their corresponding Regular Type 1 messages within repeating 10-minute transmission windows. This specification defines the data structures and identification mechanisms used to locate and correlate WSPR telemetry transmissions.

## <span id="__RefHeading___Toc2243_1057631513"></span>Core Concepts

### <span id="__RefHeading___Toc2245_1057631513"></span>Message Types

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Regular Type 1 Messages</span>**: Standard WSPR messages transmitted at the start of each 10-minute window

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Telemetry Messages</span>**: Encoded data transmissions that must be associated with their corresponding Regular messages

### <span id="__RefHeading___Toc2247_1057631513"></span>Channel Identification

Channels provide a systematic approach to locate Telemetry messages by specifying:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Unique identifier encoding (<span class="SourceText">id13</span>)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Transmission time slots

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Target frequencies

## <span id="__RefHeading___Toc2249_1057631513"></span>Data Structures

### <span id="__RefHeading___Toc2251_1057631513"></span>Channel Object

<span class="SourceText">\`\`\`</span>

<span class="SourceText">{</span>

<span class="SourceText">  "channel_number": 248,</span>

<span class="SourceText">  "id13": "12",</span>

<span class="SourceText">  "time_slot": 4,</span>

<span class="SourceText">  "frequency": 14095600,</span>

<span class="SourceText">  "band": "20m"</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2253_1057631513"></span>Telemetry Message Structure

<span class="SourceText">\`\`\`</span>

<span class="SourceText">{</span>

<span class="SourceText">  "callsign": "1X2XXX",</span>

<span class="SourceText">  "grid": "AA00",</span>

<span class="SourceText">  "power": 37,</span>

<span class="SourceText">  "frequency": 14095598,</span>

<span class="SourceText">  "timestamp": "2025-01-15T12:04:00Z",</span>

<span class="SourceText">  "id13_char1": "1",</span>

<span class="SourceText">  "id13_char3": "2"</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2255_1057631513"></span>Identification Methods

### <span id="__RefHeading___Toc2257_1057631513"></span>1. ID13 Encoding

The <span class="SourceText">id13</span> value uniquely identifies channels and is encoded into Telemetry message callsigns:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Format</span>**: Two-character identifier (00-Q9)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Encoding</span>**:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Character 1 → Callsign position 1

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Character 2 → Callsign position 3

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Purpose</span>**: Differentiates Telemetry messages sharing frequency or time slots

#### <span id="__RefHeading___Toc2259_1057631513"></span>Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">Channel 248: id13 = "12"</span>

<span class="SourceText">Blank callsign: \_ \_ \_ \_ \_ \_</span>

<span class="SourceText">After id13 encoding: 1 \_ 2 \_ \_ \_</span>

<span class="SourceText">After full encoding: 1 X 2 X X X</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2261_1057631513"></span>2. Time Slot Identification

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Definition</span>**: Specific minute within the 10-minute window when Telemetry is transmitted

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Purpose</span>**: Differentiates Telemetry messages sharing the same <span class="SourceText">id13</span> value

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Range</span>**: 0-9 minutes within each transmission window

### <span id="__RefHeading___Toc2263_1057631513"></span>3. Frequency Matching

#### <span id="__RefHeading___Toc2265_1057631513"></span>Target Frequency

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Specified in Channel Map for each channel

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Used as baseline for transmission and reception

#### <span id="__RefHeading___Toc2267_1057631513"></span>Frequency Fingerprinting, Frequency binning or other mechanisms

Due to receiver calibration issues, implement fingerprinting for accurate association:

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Locate Regular Message</span>**: Find Regular Type 1 message for target callsign

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Extract Reported Frequency</span>**: Use actual received frequency (not target frequency)

3.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Match Telemetry</span>**: Search for Telemetry messages at the reported frequency

4.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Validate Association</span>**: Confirm <span class="SourceText">id13</span> and time slot match

## <span class="SourceText">\`\`\`</span>

## <span class="SourceText"> </span>

## <span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2269_1057631513"></span>Implementation Notes

### <span id="__RefHeading___Toc2271_1057631513"></span>Receiver Calibration Challenges

Many WSPR receivers have poorly calibrated frequency references, leading to:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Inaccurate frequency reports

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Difficulty in message association

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Need for fingerprinting techniques, frequency binning, frequency binning with rx frequency error correction, or possibly even no filtering based on frequency (can have no errors, if no balloon rx spots cause conflicts on channels solely differentiated by frequency.

### <span id="__RefHeading___Toc2273_1057631513"></span>Fingerprinting Algorithm

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Baseline Establishment</span>**: Use Regular message reported frequency as reference

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Frequency Clustering</span>**: Group Telemetry messages by similar frequency deviations

3.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Temporal Correlation</span>**: Validate time slot alignment

4.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">ID13 Verification</span>**: Confirm identifier encoding matches channel specification

### <span id="__RefHeading___Toc2275_1057631513"></span>Performance Considerations

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Cache Channel Map data for frequent lookups

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Implement frequency tolerance ranges for matching

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Use time-based indexing for efficient searches

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Consider batch processing for large datasets

## <span id="__RefHeading___Toc2277_1057631513"></span>Channel Map Integration

This API integrates with the Channel Map system to provide:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Channel number to frequency mapping

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Time slot scheduling information

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>ID13 identifier assignments

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Band allocation details

Refer to the Channel Map Help documentation for detailed mapping information and scheduling specifics.

 

# <span id="__RefHeading___Toc2279_1057631513"></span>Extended Telemetry Specification

## <span id="__RefHeading___Toc2281_1057631513"></span>Overview

Extended Telemetry is an enhanced protocol that extends the Basic Telemetry scheme while maintaining full backward compatibility. It provides a flexible framework for transmitting structured telemetry data with improved encoding capabilities and extensible message types.

### <span id="__RefHeading___Toc2283_1057631513"></span>Key Features

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">16 message types</span>** including user-defined and vendor-defined types

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Up to 5 messages per 10-minute window</span>** with flexible scheduling

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Backward compatibility</span>** with Basic Telemetry and Regular Type 1 messages

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Enhanced encoding</span>** supporting up to 29.180 bits (608,212,404 values) per field

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Collision-free transmission</span>** with sender identification

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Extensible message structure</span>** for future growth

## <span id="__RefHeading___Toc2285_1057631513"></span>Message Architecture

### <span id="__RefHeading___Toc2287_1057631513"></span>Message Structure

All Extended Telemetry messages consist of two parts:

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Header Fields</span>** - Common structure across all message types

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Message Fields</span>** - Type-specific data payload

### <span id="__RefHeading___Toc2289_1057631513"></span>Header Fields

Every Extended Telemetry message includes these header fields (listed in unpacking order):

<table class="MsoNormalTable" data-border="0" data-cellspacing="0" data-cellpadding="0" width="583" style="border-collapse:collapse">
<colgroup>
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
<col style="width: 16%" />
</colgroup>
<thead>
<tr>
<th width="162" style="width: 121.2pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Field Name</p></th>
<th width="45" style="width: 33.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Type</p></th>
<th width="51" style="width: 38.0pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Range</p></th>
<th width="37" style="width: 27.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Step</p></th>
<th width="52" style="width: 38.85pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Values</p></th>
<th width="237" style="width: 177.5pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr>
<td width="162" style="width: 121.2pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p><span class="SourceText">```</span></p>
<p><span class="SourceText">HdrTelemetryType</span></p>
<p><span class="SourceText">```</span></p></td>
<td width="45" style="width: 33.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Enum</p></td>
<td width="51" style="width: 38.0pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>0-1</p></td>
<td width="37" style="width: 27.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>1</p></td>
<td width="52" style="width: 38.85pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>2</p></td>
<td width="237" style="width: 177.5pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Always 0 for Extended Telemetry</p></td>
</tr>
<tr>
<td width="162" style="width: 121.2pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p><span class="SourceText">```</span></p>
<p><span class="SourceText">HdrRESERVED</span></p>
<p><span class="SourceText">```</span></p></td>
<td width="45" style="width: 33.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Enum</p></td>
<td width="51" style="width: 38.0pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>0-3</p></td>
<td width="37" style="width: 27.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>1</p></td>
<td width="52" style="width: 38.85pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>4</p></td>
<td width="237" style="width: 177.5pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Reserved for future use (must be 0)</p></td>
</tr>
<tr>
<td width="162" style="width: 121.2pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p><span class="SourceText">```</span></p>
<p><span class="SourceText">HdrType</span></p>
<p><span class="SourceText">```</span></p></td>
<td width="45" style="width: 33.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Enum</p></td>
<td width="51" style="width: 38.0pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>0-15</p></td>
<td width="37" style="width: 27.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>1</p></td>
<td width="52" style="width: 38.85pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>16</p></td>
<td width="237" style="width: 177.5pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Message type identifier</p></td>
</tr>
<tr>
<td width="162" style="width: 121.2pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p><span class="SourceText">```</span></p>
<p><span class="SourceText">HdrSlot</span></p>
<p><span class="SourceText">```</span></p></td>
<td width="45" style="width: 33.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Enum</p></td>
<td width="51" style="width: 38.0pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>0-4</p></td>
<td width="37" style="width: 27.95pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>1</p></td>
<td width="52" style="width: 38.85pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>5</p></td>
<td width="237" style="width: 177.5pt; padding: 1.4pt 1.4pt 1.4pt 1.4pt"><p>Time slot identifier</p></td>
</tr>
</tbody>
</table>

#### <span id="__RefHeading___Toc2291_1057631513"></span>Header Field Details

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">HdrTelemetryType</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Must be set to <span class="SourceText">0</span> to identify Extended Telemetry messages

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Used to distinguish from other telemetry types

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">HdrRESERVED</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Must be set to <span class="SourceText">0b00</span>

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Reserved for future protocol extensions

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Receivers must ignore messages with non-zero values

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">HdrType</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Identifies the specific Extended Telemetry message type

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Default value: <span class="SourceText">0b0000</span>

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>See [Message Types](https://claude.ai/chat/4d21dbd6-0e7d-409e-8ab2-ab2ed59f85d8#message-types) for valid values

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">HdrSlot</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Identifies the sender and time slot (0-4)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Maps to 2-minute intervals within a 10-minute window

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Default value: <span class="SourceText">0b00</span>

## <span id="__RefHeading___Toc2293_1057631513"></span>Message Types

Extended Telemetry supports 16 different message types:

| HdrType | Type           | Description                                      |
|---------|----------------|--------------------------------------------------|
| 0       | User-Defined   | Custom structure for testing and experimentation |
| 1-14    | Enumerated     | Standardized message types (to be defined)       |
| 15      | Vendor-Defined | Vendor-specific structure and scheduling         |

### <span id="__RefHeading___Toc2295_1057631513"></span>Planned Enumerated Types (Examples)

| HdrType | Type              | Purpose                                |
|---------|-------------------|----------------------------------------|
| 1       | Basic Telemetry 2 | Extended ranges and higher resolution  |
| 2       | GPS Stats         | GPS behavior and satellite information |
| 3-14    | TBD               | Future standardized types              |

## <span id="__RefHeading___Toc2297_1057631513"></span>Time Slot Management

### <span id="__RefHeading___Toc2299_1057631513"></span>10-Minute Window Structure

Extended Telemetry operates within established 10-minute transmission windows, divided into 5 time slots:

| Slot | Timing        | Usage          |
|------|---------------|----------------|
| 0    | Start minute  | Primary slot   |
| 1    | Start + 2 min | Secondary slot |
| 2    | Start + 4 min | Extended slot  |
| 3    | Start + 6 min | Extended slot  |
| 4    | Start + 8 min | Extended slot  |

### <span id="__RefHeading___Toc2301_1057631513"></span>Transmission Patterns

Extended Telemetry provides flexible transmission patterns:

#### <span id="__RefHeading___Toc2303_1057631513"></span>Backward Compatible

<span class="SourceText">\`\`\`</span>

<span class="SourceText">Slot 0: Regular Type 1</span>

<span class="SourceText">Slot 1: Basic Telemetry</span>

<span class="SourceText">Slots 2-4: \[Available for Extended Telemetry\]</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2305_1057631513"></span>Extended Only

<span class="SourceText">\`\`\`</span>

<span class="SourceText">Slots 0-4: \[Extended Telemetry in any combination\]</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2307_1057631513"></span>Mixed Mode

<span class="SourceText">\`\`\`</span>

<span class="SourceText">Slot 0: Regular Type 1</span>

<span class="SourceText">Slot 1: Extended Telemetry (replacing Basic)</span>

<span class="SourceText">Slots 2-4: Extended Telemetry</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2309_1057631513"></span>Encoding Specification

### <span id="__RefHeading___Toc2311_1057631513"></span>Data Encoding

Extended Telemetry uses a unified encoding algorithm that:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Supports field values up to 29.180 bits (608,212,404 values)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Allows fields to span the entire WSPR message space

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Implements defined clamping and rounding behaviors

### <span id="__RefHeading___Toc2313_1057631513"></span>Packing Order

Fields are packed into the big number in **<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">reverse order</span>** from their definition:

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>Message fields (last defined → first defined)

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>Header fields (HdrSlot → HdrType → HdrRESERVED → HdrTelemetryType)

### <span id="__RefHeading___Toc2315_1057631513"></span>Value Processing

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Clamping Behavior</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>No rollover occurs

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>All values are clamped to their defined ranges before encoding

**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Rounding Behavior</span>**

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Field values are rounded to the closest multiple of step size within range

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Rounding occurs during encoding process

## <span id="__RefHeading___Toc2317_1057631513"></span>Example Implementation

### <span id="__RefHeading___Toc2319_1057631513"></span>GPS Stats Message (Hypothetical)

<span class="SourceText">\`\`\`</span>

<span class="SourceText">Message Type: GPS Stats (HdrType = 2)</span>

<span class="SourceText"> </span>

<span class="SourceText">Field Definitions:</span>

<span class="SourceText">- SatsUSA: 0-128, step 4 (33 values, 5.044 bits)</span>

<span class="SourceText">- SatsChina: 0-128, step 4 (33 values, 5.044 bits)</span>

<span class="SourceText">- SatsRussia: 0-128, step 4 (33 values, 5.044 bits)</span>

<span class="SourceText">- SatsEU: 0-128, step 4 (33 values, 5.044 bits)</span>

<span class="SourceText">- SatsIndia: 0-128, step 4 (33 values, 5.044 bits)</span>

<span class="SourceText">- hdop: 0-10, step 2 (6 values, 2.585 bits)</span>

<span class="SourceText"> </span>

<span class="SourceText">Encoding Analysis:</span>

<span class="SourceText">- Available bits: 29.180</span>

<span class="SourceText">- Used bits: 27.807 (95.29%)</span>

<span class="SourceText">- Remaining bits: 1.373 (4.71%)</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2321_1057631513"></span>Packing Example

For GPS Stats message, packing order would be:

<span class="SourceText">\`\`\`</span>

<span class="SourceText">1. hdop (message field - last defined)</span>

<span class="SourceText">2. SatsIndia</span>

<span class="SourceText">3. SatsEU</span>

<span class="SourceText">4. SatsRussia</span>

<span class="SourceText">5. SatsChina</span>

<span class="SourceText">6. SatsUSA (message field - first defined)</span>

<span class="SourceText">7. HdrSlot (header field)</span>

<span class="SourceText">8. HdrType</span>

<span class="SourceText">9. HdrRESERVED</span>

<span class="SourceText">10. HdrTelemetryType (header field - first)</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2323_1057631513"></span>Integration Guidelines

### <span id="__RefHeading___Toc2325_1057631513"></span>Receiver Implementation

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Message Detection</span>**: Check HdrTelemetryType = 0

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Version Compatibility</span>**: Ignore messages with HdrRESERVED ≠ 0

3.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Type Handling</span>**: Use HdrType to determine message structure

4.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Slot Management</span>**: Use HdrSlot for sender identification

### <span id="__RefHeading___Toc2327_1057631513"></span>Sender Implementation

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Header Setup</span>**: Always set HdrTelemetryType = 0, HdrRESERVED = 0

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Type Selection</span>**: Choose appropriate HdrType for message content

3.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Slot Assignment</span>**: Select HdrSlot based on transmission schedule

4.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Value Processing</span>**: Apply clamping and rounding before encoding

### <span id="__RefHeading___Toc2329_1057631513"></span>Fingerprinting Logic

For websites that use a variety of “fingerprinting” algos, it is useful to be similar for deciding how to fingerprint when Basic and Extended Telemetry exists.

For telemetry detection in any 10-minute window:

1.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>Check slot 0 for both Regular and Extended messages

2.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>If only Regular found: use as reference frequency

3.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>If only Extended found: use as reference frequency

4.<span style="font:7.0pt &quot;Times New Roman&quot;">    </span>If both found: prefer Regular message as reference

## <span id="__RefHeading___Toc2331_1057631513"></span>Error Handling

### <span id="__RefHeading___Toc2333_1057631513"></span>Invalid Messages

Receivers should ignore messages with:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>HdrTelemetryType ≠ 0

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>HdrRESERVED ≠ 0

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Unknown HdrType values (beyond implemented range)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Invalid field values outside defined ranges

### <span id="__RefHeading___Toc2335_1057631513"></span>Backward Compatibility

Extended Telemetry maintains compatibility by:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Using existing WSPR message format

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Preserving Regular Type 1 and Basic Telemetry timing

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Not interfering with existing transmission patterns

## <span id="__RefHeading___Toc2337_1057631513"></span>Future Extensions

The protocol supports future growth through:

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Extensible message types (add fields to existing types)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>HdrRESERVED field for protocol enhancements

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>User-defined and vendor-defined message types

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Flexible transmission scheduling

 

# <span id="__RefHeading___Toc2339_1057631513"></span>WsprEncoded C++ Library

## <span id="__RefHeading___Toc2341_1057631513"></span>Overview

WsprEncoded is a header-only C++ library that implements telemetry encoding and decoding functionality for the WSPR (Weak Signal Propagation Reporter) protocol. This library enables developers to build trackers and other telemetry systems that can transmit sensor data through WSPR's minimal bandwidth constraints.

## <span id="__RefHeading___Toc2343_1057631513"></span>Features

### <span id="__RefHeading___Toc2345_1057631513"></span>Core Capabilities

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Basic Telemetry</span>**: Encode/decode common measurements (altitude, voltage, temperature, etc.)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Extended Telemetry</span>**: Define and encode arbitrary telemetry fields

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Channel Mapping</span>**: Look up WSPR channel details by band and frequency

### <span id="__RefHeading___Toc2347_1057631513"></span>Design Principles

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Memory Efficient</span>**: No dynamic memory allocations (<span class="SourceText">malloc</span>, <span class="SourceText">new</span>, or STL containers)

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Widely Compatible</span>**: C++11 language standard for older compiler support

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Header-Only</span>**: Simple integration without separate compilation

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Cross-Platform</span>**: Works on Arduino, embedded systems, and desktop platforms

## <span id="__RefHeading___Toc2349_1057631513"></span>Installation

### <span id="__RefHeading___Toc2351_1057631513"></span>Arduino Library Manager

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\# Install via Arduino IDE Library Manager</span>

<span class="SourceText">\# Search for "WsprEncoded" and click Install</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2353_1057631513"></span>CMake Integration

#### <span id="__RefHeading___Toc2355_1057631513"></span>Option 1: FetchContent (Recommended)

<span class="SourceText">\`\`\`</span>

<span class="SourceText">include(FetchContent)</span>

<span class="SourceText">FetchContent_Declare(</span>

<span class="SourceText">  WsprEncoded</span>

<span class="SourceText">  GIT_REPOSITORY https://github.com/your-repo/WsprEncoded.git</span>

<span class="SourceText">  GIT_TAG        v1.0.0</span>

<span class="SourceText">)</span>

<span class="SourceText">FetchContent_MakeAvailable(WsprEncoded)</span>

<span class="SourceText"> </span>

<span class="SourceText">target_link_libraries(YourExecutable WsprEncoded)</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2357_1057631513"></span>Option 2: Git Submodules

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\# Add as submodule</span>

<span class="SourceText">git submodule add https://github.com/your-repo/WsprEncoded.git third-party/WsprEncoded</span>

<span class="SourceText"> </span>

<span class="SourceText">\# In CMakeLists.txt</span>

<span class="SourceText">add_subdirectory(third-party/WsprEncoded)</span>

<span class="SourceText">target_link_libraries(YourExecutable WsprEncoded)</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2359_1057631513"></span>Option 3: External Directory

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\# If WsprEncoded is in a sibling directory</span>

<span class="SourceText">add_subdirectory(../WsprEncoded WsprEncoded)</span>

<span class="SourceText">target_link_libraries(YourExecutable WsprEncoded)</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2361_1057631513"></span>API Reference

### <span id="__RefHeading___Toc2363_1057631513"></span>Core Headers

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/TelemetryBasic.h\>      // Basic telemetry types</span>

<span class="SourceText">\#include \<WsprEncoded/TelemetryExtended.h\>   // User-defined telemetry</span>

<span class="SourceText">\#include \<WsprEncoded/ChannelMap.h\>          // Channel mapping utilities</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2365_1057631513"></span>Basic Telemetry API

#### <span id="__RefHeading___Toc2367_1057631513"></span>Common Measurement Types

<span class="SourceText">\`\`\`</span>

<span class="SourceText">namespace WsprEncoded {</span>

<span class="SourceText">    // Predefined measurement types</span>

<span class="SourceText">    struct AltitudeMeasurement {</span>

<span class="SourceText">        static constexpr uint16_t min_value = 0;</span>

<span class="SourceText">        static constexpr uint16_t max_value = 21000;  // meters</span>

<span class="SourceText">        static constexpr uint16_t resolution = 20;     // 20m steps</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    struct VoltageMeasurement {</span>

<span class="SourceText">        static constexpr uint16_t min_value = 0;</span>

<span class="SourceText">        static constexpr uint16_t max_value = 5000;    // millivolts</span>

<span class="SourceText">        static constexpr uint16_t resolution = 10;     // 10mV steps</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    struct TemperatureMeasurement {</span>

<span class="SourceText">        static constexpr int16_t min_value = -40;</span>

<span class="SourceText">        static constexpr int16_t max_value = 80;       // celsius</span>

<span class="SourceText">        static constexpr uint16_t resolution = 1;      // 1°C steps</span>

<span class="SourceText">    };</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2369_1057631513"></span>Encoding Functions

<span class="SourceText">\`\`\`</span>

<span class="SourceText">class BasicTelemetryEncoder {</span>

<span class="SourceText">public:</span>

<span class="SourceText">    // Encode single measurement</span>

<span class="SourceText">    template\<typename MeasurementType\></span>

<span class="SourceText">    static bool encode(uint16_t value, uint8_t& encoded_index);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Encode multiple measurements into WSPR message</span>

<span class="SourceText">    static bool encodeToWSPR(</span>

<span class="SourceText">        const uint16_t\* values,</span>

<span class="SourceText">        const uint8_t\* measurement_types,</span>

<span class="SourceText">        uint8_t count,</span>

<span class="SourceText">        WSPRMessage& message</span>

<span class="SourceText">    );</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Decode from WSPR message</span>

<span class="SourceText">    static bool decodeFromWSPR(</span>

<span class="SourceText">        const WSPRMessage& message,</span>

<span class="SourceText">        uint16_t\* values,</span>

<span class="SourceText">        uint8_t\* measurement_types,</span>

<span class="SourceText">        uint8_t& count</span>

<span class="SourceText">    );</span>

<span class="SourceText">};</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2371_1057631513"></span>Usage Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/TelemetryBasic.h\></span>

<span class="SourceText"> </span>

<span class="SourceText">void encodeBasicTelemetry() {</span>

<span class="SourceText">    using namespace WsprEncoded;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Prepare measurements</span>

<span class="SourceText">    uint16_t altitude = 1200;  // meters</span>

<span class="SourceText">    uint16_t voltage = 3300;   // millivolts</span>

<span class="SourceText">    int16_t temperature = 25;  // celsius</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Create encoder</span>

<span class="SourceText">    BasicTelemetryEncoder encoder;</span>

<span class="SourceText">    WSPRMessage message;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Encode measurements</span>

<span class="SourceText">    uint16_t values\[\] = {altitude, voltage, temperature};</span>

<span class="SourceText">    uint8_t types\[\] = {</span>

<span class="SourceText">        MeasurementType::ALTITUDE,</span>

<span class="SourceText">        MeasurementType::VOLTAGE,</span>

<span class="SourceText">        MeasurementType::TEMPERATURE</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    if (encoder.encodeToWSPR(values, types, 3, message)) {</span>

<span class="SourceText">        // Success - message ready for transmission</span>

<span class="SourceText">        printf("Encoded WSPR: %s %s %d\n", </span>

<span class="SourceText">               message.callsign, message.grid, message.power);</span>

<span class="SourceText">    }</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2373_1057631513"></span>Extended Telemetry API

#### <span id="__RefHeading___Toc2375_1057631513"></span>Custom Field Definition

<span class="SourceText">\`\`\`</span>

<span class="SourceText">class ExtendedTelemetryEncoder {</span>

<span class="SourceText">public:</span>

<span class="SourceText">    // Define custom measurement field</span>

<span class="SourceText">    struct FieldDefinition {</span>

<span class="SourceText">        uint16_t min_value;</span>

<span class="SourceText">        uint16_t max_value;</span>

<span class="SourceText">        uint16_t resolution;</span>

<span class="SourceText">        uint8_t bit_count;</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Add field to encoder</span>

<span class="SourceText">    bool addField(const FieldDefinition& field);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Encode custom telemetry</span>

<span class="SourceText">    bool encode(const uint16_t\* values, uint8_t count, WSPRMessage& message);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Decode custom telemetry</span>

<span class="SourceText">    bool decode(const WSPRMessage& message, uint16_t\* values, uint8_t& count);</span>

<span class="SourceText">};</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2377_1057631513"></span>Custom Telemetry Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/TelemetryExtended.h\></span>

<span class="SourceText"> </span>

<span class="SourceText">void encodeCustomTelemetry() {</span>

<span class="SourceText">    using namespace WsprEncoded;</span>

<span class="SourceText">    </span>

<span class="SourceText">    ExtendedTelemetryEncoder encoder;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Define custom pressure field (800-1200 hPa, 1 hPa resolution)</span>

<span class="SourceText">    ExtendedTelemetryEncoder::FieldDefinition pressure_field = {</span>

<span class="SourceText">        .min_value = 800,</span>

<span class="SourceText">        .max_value = 1200,</span>

<span class="SourceText">        .resolution = 1,</span>

<span class="SourceText">        .bit_count = 9  // 2^9 = 512 values (enough for 400 hPa range)</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Define custom humidity field (0-100%, 1% resolution)</span>

<span class="SourceText">    ExtendedTelemetryEncoder::FieldDefinition humidity_field = {</span>

<span class="SourceText">        .min_value = 0,</span>

<span class="SourceText">        .max_value = 100,</span>

<span class="SourceText">        .resolution = 1,</span>

<span class="SourceText">        .bit_count = 7  // 2^7 = 128 values (enough for 100% range)</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Add fields to encoder</span>

<span class="SourceText">    encoder.addField(pressure_field);</span>

<span class="SourceText">    encoder.addField(humidity_field);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Encode measurements</span>

<span class="SourceText">    uint16_t values\[\] = {1013, 65};  // 1013 hPa, 65% humidity</span>

<span class="SourceText">    WSPRMessage message;</span>

<span class="SourceText">    </span>

<span class="SourceText">    if (encoder.encode(values, 2, message)) {</span>

<span class="SourceText">        // Success - custom telemetry encoded</span>

<span class="SourceText">        printf("Custom telemetry encoded successfully\n");</span>

<span class="SourceText">    }</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2379_1057631513"></span>Channel Map API

#### <span id="__RefHeading___Toc2381_1057631513"></span>Channel Information

<span class="SourceText">\`\`\`</span>

<span class="SourceText">class ChannelMap {</span>

<span class="SourceText">public:</span>

<span class="SourceText">    struct ChannelInfo {</span>

<span class="SourceText">        uint8_t channel_id;</span>

<span class="SourceText">        uint8_t start_minute;     // Minute within 2-hour window</span>

<span class="SourceText">        uint32_t frequency_hz;    // Exact frequency in Hz</span>

<span class="SourceText">        uint8_t band;            // Amateur radio band</span>

<span class="SourceText">    };</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Get channel info by band and channel</span>

<span class="SourceText">    static bool getChannelInfo(uint8_t band, uint8_t channel, ChannelInfo& info);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Get all channels for a band</span>

<span class="SourceText">    static uint8_t getChannelsForBand(uint8_t band, ChannelInfo\* channels, uint8_t max_count);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Find optimal channel for current time</span>

<span class="SourceText">    static bool findOptimalChannel(uint8_t band, uint8_t current_minute, ChannelInfo& info);</span>

<span class="SourceText">};</span>

<span class="SourceText">\`\`\`</span>

#### <span id="__RefHeading___Toc2383_1057631513"></span>Channel Map Example

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/ChannelMap.h\></span>

<span class="SourceText"> </span>

<span class="SourceText">void useChannelMap() {</span>

<span class="SourceText">    using namespace WsprEncoded;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Get 20m band, channel 13 information</span>

<span class="SourceText">    ChannelMap::ChannelInfo info;</span>

<span class="SourceText">    if (ChannelMap::getChannelInfo(20, 13, info)) {</span>

<span class="SourceText">        printf("Channel 13: Start minute %d, Frequency %lu Hz\n", </span>

<span class="SourceText">               info.start_minute, info.frequency_hz);</span>

<span class="SourceText">    }</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Find optimal channel for current time (assuming minute 15)</span>

<span class="SourceText">    ChannelMap::ChannelInfo optimal;</span>

<span class="SourceText">    if (ChannelMap::findOptimalChannel(20, 15, optimal)) {</span>

<span class="SourceText">        printf("Optimal channel: %d at %lu Hz\n", </span>

<span class="SourceText">               optimal.channel_id, optimal.frequency_hz);</span>

<span class="SourceText">    }</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2385_1057631513"></span>Complete Integration Example

### <span id="__RefHeading___Toc2387_1057631513"></span>Arduino Tracker Implementation

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/TelemetryBasic.h\></span>

<span class="SourceText">\#include \<WsprEncoded/ChannelMap.h\></span>

<span class="SourceText"> </span>

<span class="SourceText">class WSPRTracker {</span>

<span class="SourceText">private:</span>

<span class="SourceText">    WsprEncoded::BasicTelemetryEncoder encoder;</span>

<span class="SourceText">    WsprEncoded::ChannelMap channelMap;</span>

<span class="SourceText">    </span>

<span class="SourceText">public:</span>

<span class="SourceText">    bool transmitTelemetry(uint16_t altitude, uint16_t voltage, int16_t temp) {</span>

<span class="SourceText">        // Encode telemetry</span>

<span class="SourceText">        WsprEncoded::WSPRMessage message;</span>

<span class="SourceText">        uint16_t values\[\] = {altitude, voltage, temp};</span>

<span class="SourceText">        uint8_t types\[\] = {</span>

<span class="SourceText">            WsprEncoded::MeasurementType::ALTITUDE,</span>

<span class="SourceText">            WsprEncoded::MeasurementType::VOLTAGE,</span>

<span class="SourceText">            WsprEncoded::MeasurementType::TEMPERATURE</span>

<span class="SourceText">        };</span>

<span class="SourceText">        </span>

<span class="SourceText">        if (!encoder.encodeToWSPR(values, types, 3, message)) {</span>

<span class="SourceText">            return false;</span>

<span class="SourceText">        }</span>

<span class="SourceText">        </span>

<span class="SourceText"> </span>

<span class="SourceText">        // Find optimal transmission channel. </span>

<span class="SourceText">        // Usually a tracker will be configured to use a single channel.</span>

<span class="SourceText">        WsprEncoded::ChannelMap::ChannelInfo channel;</span>

<span class="SourceText">        uint8_t current_minute = getCurrentMinute();</span>

<span class="SourceText">        </span>

<span class="SourceText">        if (!channelMap.findOptimalChannel(20, current_minute, channel)) {</span>

<span class="SourceText">            return false;</span>

<span class="SourceText">        }</span>

<span class="SourceText">        </span>

<span class="SourceText">        // Transmit WSPR message</span>

<span class="SourceText">        return transmitWSPR(message, channel.frequency_hz);</span>

<span class="SourceText">    }</span>

<span class="SourceText">    </span>

<span class="SourceText">private:</span>

<span class="SourceText">    bool transmitWSPR(const WsprEncoded::WSPRMessage& msg, uint32_t freq) {</span>

<span class="SourceText">        // Platform-specific WSPR transmission implementation</span>

<span class="SourceText">        // ...</span>

<span class="SourceText">        return true;</span>

<span class="SourceText">    }</span>

<span class="SourceText">    </span>

<span class="SourceText">    uint8_t getCurrentMinute() {</span>

<span class="SourceText">        // Get current minute within 2-hour WSPR window</span>

<span class="SourceText">        // ...</span>

<span class="SourceText">        return 0;</span>

<span class="SourceText">    }</span>

<span class="SourceText">};</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2389_1057631513"></span>Desktop Application Integration

<span class="SourceText">\`\`\`</span>

<span class="SourceText">\#include \<WsprEncoded/TelemetryExtended.h\></span>

<span class="SourceText">\#include \<iostream\></span>

<span class="SourceText"> </span>

<span class="SourceText">int main() {</span>

<span class="SourceText">    using namespace WsprEncoded;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Create extended telemetry encoder for weather station</span>

<span class="SourceText">    ExtendedTelemetryEncoder encoder;</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Define weather measurements</span>

<span class="SourceText">    ExtendedTelemetryEncoder::FieldDefinition pressure = {800, 1200, 1, 9};</span>

<span class="SourceText">    ExtendedTelemetryEncoder::FieldDefinition humidity = {0, 100, 1, 7};</span>

<span class="SourceText">    ExtendedTelemetryEncoder::FieldDefinition wind_speed = {0, 200, 1, 8};</span>

<span class="SourceText">    </span>

<span class="SourceText">    encoder.addField(pressure);</span>

<span class="SourceText">    encoder.addField(humidity);</span>

<span class="SourceText">    encoder.addField(wind_speed);</span>

<span class="SourceText">    </span>

<span class="SourceText">    // Simulate weather readings</span>

<span class="SourceText">    uint16_t readings\[\] = {1013, 65, 12};  // 1013 hPa, 65%, 12 km/h</span>

<span class="SourceText">    WSPRMessage message;</span>

<span class="SourceText">    </span>

<span class="SourceText">    if (encoder.encode(readings, 3, message)) {</span>

<span class="SourceText">        std::cout \<\< "Weather telemetry encoded: " </span>

<span class="SourceText">                  \<\< message.callsign \<\< " " \<\< message.grid \<\< " " \<\< message.power </span>

<span class="SourceText">                  \<\< std::endl;</span>

<span class="SourceText">    }</span>

<span class="SourceText">    </span>

<span class="SourceText">    return 0;</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

## <span id="__RefHeading___Toc2391_1057631513"></span>Error Handling

### <span id="__RefHeading___Toc2393_1057631513"></span>Common Error Codes

<span class="SourceText">\`\`\`</span>

<span class="SourceText">namespace WsprEncoded {</span>

<span class="SourceText">    enum class ErrorCode {</span>

<span class="SourceText">        SUCCESS = 0,</span>

<span class="SourceText">        INVALID_RANGE,          // Value outside measurement range</span>

<span class="SourceText">        INSUFFICIENT_BITS,      // Not enough bits for encoding</span>

<span class="SourceText">        DECODE_FAILED,          // Decoding operation failed</span>

<span class="SourceText">        INVALID_CHANNEL,        // Channel not found</span>

<span class="SourceText">        MEMORY_FULL             // No more fields can be added</span>

<span class="SourceText">    };</span>

<span class="SourceText">}</span>

<span class="SourceText">\`\`\`</span>

### <span id="__RefHeading___Toc2395_1057631513"></span>Best Practices

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Always check return values from encoding/decoding functions

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Validate measurement values are within defined ranges

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Handle bit capacity limitations gracefully

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Use appropriate measurement resolutions to optimize data usage

## <span id="__RefHeading___Toc2397_1057631513"></span>Performance Notes

### <span id="__RefHeading___Toc2399_1057631513"></span>Memory Usage

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Header-only library adds minimal overhead

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>No dynamic allocations - all memory usage is compile-time determined

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Typical memory footprint: \< 1KB for basic telemetry, \< 2KB for extended

### <span id="__RefHeading___Toc2401_1057631513"></span>Processing Speed

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Encoding/decoding operations are O(n) where n is number of measurements

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Optimized for embedded systems with limited CPU resources

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>Typical encoding time: \< 1ms on Arduino-class processors

## <span id="__RefHeading___Toc2403_1057631513"></span>Platform Support

### <span id="__RefHeading___Toc2405_1057631513"></span>Tested Platforms

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Arduino</span>**: Uno, Nano, ESP32, ESP8266

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Desktop</span>**: Windows, Linux, macOS

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Embedded</span>**: ARM Cortex-M, AVR, PIC32

### <span id="__RefHeading___Toc2407_1057631513"></span>Compiler Requirements

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Minimum</span>**: C++11 support

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Recommended</span>**: C++14 or later for better template support

<span style="font-family:Symbol">·<span style="font:7.0pt &quot;Times New Roman&quot;">      </span></span>**<span style="font-family:&quot;Liberation Serif&quot;,sans-serif">Tested</span>**: GCC 4.9+, Clang 3.5+, MSVC 2015+

 

 

 

 

 

</div>
