TMD-26507 Verify the values of Effective Power and Potential Power fields for Cooling Unit
## Test Steps
On a Cooling unit with 5 Power ports and N+1 redundancy. The ports should be, for example, Single Phase (3-wire), 120-240 volts, IEC-320-C14 connector, Watts (N) = 55, Watts(B) = 33. The important number for calculations is the last one, Watts(B)=33. If you make different ports, note that number. Test these combinations:

1. Initial state: no connected ports
2. Mark one port as "In Use"
3. Mark another port as "In Use"
4. One of the "In Use" ports, connect it to a real item.
5. Make the Redundancy to be N, not N+1

## Test Results
1. EP=0, PP=132
2. EP=33, PP=132
3. EP=66, PP=132
4. EP=66, PP=132
5. EP=66, PP=165
The fields and values are shown in the Items List also.