
# AMD Vanilla Clover Patches

## Patches to enable Native AMD CPU Support on 10.13.6 and 10.14.x

 - Beta 
 - Support Currently only supports Ryzen CPUs
 -  Enables the use of iMessage, Siri etc
 
 
 ### Clover KernelToPatch


		<key>KernelToPatch</key>
		<array>
			<dict>
				<key>Comment</key>
				<string>algrey - commpage_populate -remove rdmsr</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				uaABAAAPMg==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				Dx+AAAAAAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpu_topology_sort -disable _x86_validate_topology</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				6Ar2//+c
				</data>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				Dx9EAACc
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpu_topology_sort -disable _x86_validate_topology</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				6Kn1//8=
				</data>
				<key>MatchOS</key>
				<string>10.14.1,10.14.2,10.14.3</string>
				<key>Replace</key>
				<data>
				Dx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpu_topology_sort -disable _x86_validate_topology</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				6Jn1//8=
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				Dx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - cpuid 0x8000001D instead 0</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				McAx2zHJMdIPokGJxkGJ0YM9ygWNAAB0GEiNPZKSXwAx
				9jHAQYnIRInyidno6IlYAEGD/gQPgvoBAABFMfbrDGYP
				H4QAAAAAAA==
				</data>
				<key>MatchBuild</key>
				<string>17G65,17G66</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				uB0AAIAx2zHJMdIPokGJxkGJ0YM9xwWNAAB0G0iNPY+S
				XwC+HQAAgDHAQYnIRInyidno4olYAEGD/gQPgvQBAABF
				MfbrBg8fAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - cpuid 0x8000001D instead 0</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				McAx2zHJMdIPokGJxkGJ0YM9yu2MAAB0GEiNPQ+GXwAx
				9jHAQYnIRInyidno2HpYAEGD/gQPgvoBAABFMfbrDGYP
				H4QAAAAAAA==
				</data>
				<key>MatchBuild</key>
				<string>17G5019</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				uB0AAIAx2zHJMdIPokGJxkGJ0YM9x+2MAAB0G0iNPQyG
				XwC+HQAAgDHAQYnIRInyidno0npYAEGD/gQPgvQBAABF
				MfbrBg8fAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - cpuid 0x8000001D instead 0</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				McAx2zHJMdIPokGJxkGJ0YM9+kGYAAB0GEiNPSvZZwAx
				9jHAQYnIRInyidno2CxgAEGD/gQPgvsBAABFMfbrDGYP
				H4QAAAAAAA==
				</data>
				<key>MatchOS</key>
				<string>10.14.1</string>
				<key>Replace</key>
				<data>
				uB0AAIAx2zHJMdIPokGJxkGJ0YM990GYAAB0G0iNPSjZ
				ZwC+HQAAgDHAQYnIRInyidno0ixgAEGD/gQPgvUBAABF
				MfbrBg8fAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - cpuid 0x8000001D instead 0</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				McAx2zHJMdIPokGJxkGJ0YM9SiSYAAB0GEiNPQvGZwAx
				9jHAQYnIRInyidnoWBpgAEGD/gQPgvsBAABFMfbrDGYP
				H4QAAAAAAA==
				</data>
				<key>MatchOS</key>
				<string>10.14.3</string>
				<key>Replace</key>
				<data>
				uB0AAIAx2zHJMdIPokGJxkGJ0YM9RySYAAB0G0iNPQjG
				ZwC+HQAAgDHAQYnIRInyidnoUhpgAEGD/gQPgvUBAABF
				MfbrBg8fAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - cpuid 0x8000001D instead 0</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				McAx2zHJMdIPokGJxoM9re2XAAB0G0GJ0UiNPRehZwAx
				9jHAQYnIRInyidnoWP1fAEGD/gQPgvgBAABFMfbrDGYP
				H4QAAAAAAA==
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				uB0AAIAx2zHJMdIPokGJxkGJ0YM9p+2XAAB0G0iNPRSh
				ZwC+HQAAgDHAQYnIRInyidnoUv1fAEGD/gQPgvUBAABF
				MfbrBg8fAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - cpuid 0x8000001D instead 4</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				uAQAAABEifFEiQ==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				uB0AAIBEifFEiQ==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - don't set cpuid_cores_per_package</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				wega/8CJBRgEjQBEieg=
				</data>
				<key>MatchBuild</key>
				<string>17G65,17G66</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				Zg8fhAAAAAAADx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - don't set cpuid_cores_per_package</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				wega/8CJBRjsjABEieg=
				</data>
				<key>MatchBuild</key>
				<string>17G5019</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				Zg8fhAAAAAAADx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - don't set cpuid_cores_per_package</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				wega/8CJBUhAmABEieg=
				</data>
				<key>MatchOS</key>
				<string>10.14.1</string>
				<key>Replace</key>
				<data>
				Zg8fhAAAAAAADx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - don't set cpuid_cores_per_package</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				wega/8CJBZgimABEieg=
				</data>
				<key>MatchOS</key>
				<string>10.14.3</string>
				<key>Replace</key>
				<data>
				Zg8fhAAAAAAADx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cache_info - don't set cpuid_cores_per_package</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				wega/8A=
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				Dx8A6wY=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_generic_info - remove wrmsr</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				uYsAAAAxwDHSDzA=
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				Zg8fhAAAAAAAZpA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_generic_info - set microcode=186</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				uYsAAAAPMg==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				uroAAABmkA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_generic_info - set flag=1</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				uRcAAAAPMsHqEoDiBw==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				sgFmDx+EAAAAAABmkA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_generic_info - disable check to allow leaf7</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				ADoPgg==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				AAAPgg==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_info - GenuineIntel to AuthenticAMD </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				R2VudWluZUludGVsAA==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				QXV0aGVudGljQU1EAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cpufamily - force CPUFAMILY_INTEL_SKYLAKE </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				MduAPbgLjQAGdVw=
				</data>
				<key>MatchBuild</key>
				<string>17G65,17G66</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				u58h/DfpXQAAAJA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cpufamily - force CPUFAMILY_INTEL_SKYLAKE </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				MduAPbjzjAAGdVw=
				</data>
				<key>MatchBuild</key>
				<string>17G5019</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				u58h/DfpXQAAAJA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cpufamily - force CPUFAMILY_INTEL_SKYLAKE </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				MduAPehHmAAGdVw=
				</data>
				<key>MatchOS</key>
				<string>10.14.1</string>
				<key>Replace</key>
				<data>
				u58h/DfpXQAAAJA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cpufamily - force CPUFAMILY_INTEL_SKYLAKE </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				MduAPTgqmAAGdVw=
				</data>
				<key>MatchOS</key>
				<string>10.14.3</string>
				<key>Replace</key>
				<data>
				u58h/DfpXQAAAJA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_cpufamily - force CPUFAMILY_INTEL_SKYLAKE </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				MduAPZjzlwAGdVw=
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				u58h/DfpXQAAAJA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_info - ryzen cores and logicals count</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				PexeO1d0Gz28T+p4dTaLBcgKjQCJBYoLjQCLDcAKjQDr
				Frk1AAAADzIPt8jB6BCD4A+JBWwLjQCJDWoLjQCFwHVK
				6zC5NQAAAA8ySMHiIInBSAnRuQEAAQAPRcgPt9GJyMHo
				EIkFOguNAIkVOAuNAIXAdRiLBWIKjQCJBSQLjQCLBVoK
				jQCJBRwLjQA=
				</data>
				<key>MatchBuild</key>
				<string>17G65,17G66</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				uAgAAIAx2zHJMdIPokGJwEGJzkGJ0YM97wuNAAB0G2YP
				H4QAAAAAAGYPH4QAAAAAAGYPH4QAAAAAAEUPtvZB/8a4
				HgAAgDHbMckx0g+iQYnAQYnRZg8fhAAAAAAAD7bP/8Ex
				0kSJ8PfxiQVtCo0ARIk1agqNAIM9JwuNAAB1DYkFHwuN
				AESJNRwLjQA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_info - ryzen cores and logicals count</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				PexeO1d0Gz28T+p4dTaLBcjyjACJBYrzjACLDcDyjADr
				Frk1AAAADzIPt8jB6BCD4A+JBWzzjACJDWrzjACFwHVK
				6zC5NQAAAA8ySMHiIInBSAnRuQEAAQAPRcgPt9GJyMHo
				EIkFOvOMAIkVOPOMAIXAdRiLBWLyjACJBSTzjACLBVry
				jACJBRzzjAA=
				</data>
				<key>MatchBuild</key>
				<string>17G5019</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				uAgAAIAx2zHJMdIPokGJwEGJzkGJ0YM97/OMAAB0G2YP
				H4QAAAAAAGYPH4QAAAAAAGYPH4QAAAAAAEUPtvZB/8a4
				HgAAgDHbMckx0g+iQYnAQYnRZg8fhAAAAAAAD7bP/8Ex
				0kSJ8PfxiQVt8owARIk1avKMAIM9J/OMAAB1DYkFH/OM
				AESJNRzzjAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_info - ryzen cores and logicals count</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				PexeO1d0Gz28T+p4dSaLBfhGmACJBbpHmACLDfBGmADr
				OLk1AAAADzIPt8jB6BCD4A/rILk1AAAADzJIweIgicFI
				CdG6AQABAA9F0A+3yonQwegQiQV6R5gAiQ14R5gAhcB0
				Gg==
				</data>
				<key>MatchOS</key>
				<string>10.14.1</string>
				<key>Replace</key>
				<data>
				uAgAAIAx2zHJMdIPokGJwEGJzkGJ0UUPtvZB/8a4HgAA
				gDHbMckx0g+iQYnAQYnRDx9EAAAPts//wTHSRInw9/GJ
				BcVGmABEiTXCRpgAgz1/R5gAAHUNiQV3R5gARIk1dEeY
				AA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_info - ryzen cores and logicals count</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				PexeO1d0Gz28T+p4dSaLBUgpmACJBQoqmACLDUApmADr
				OLk1AAAADzIPt8jB6BCD4A/rILk1AAAADzJIweIgicFI
				CdG6AQABAA9F0A+3yonQwegQiQXKKZgAiQ3IKZgAhcB0
				Gg==
				</data>
				<key>MatchOS</key>
				<string>10.14.3</string>
				<key>Replace</key>
				<data>
				uAgAAIAx2zHJMdIPokGJwEGJzkGJ0UUPtvZB/8a4HgAA
				gDHbMckx0g+iQYnAQYnRDx9EAAAPts//wTHSRInw9/GJ
				BRUpmABEiTUSKZgAgz3PKZgAAHUNiQXHKZgARIk1xCmY
				AA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpuid_set_info - ryzen cores and logicals count</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				PexeO1d0Gz28T+p4dSaLBafylwCJBWnzlwCLDZ/ylwDr
				OLk1AAAADzIPt8jB6BCD4A/rILk1AAAADzJIweIgicFI
				CdG6AQABAA9F0A+3yonQwegQiQUp85cAiQ0n85cAhcB0
				Gg==
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				uAgAAIAx2zHJMdIPokGJwEGJzkGJ0UUPtvZB/8a4HgAA
				gDHbMckx0g+iQYnAQYnRDx9EAAAPts//wTHSRInw9/GJ
				BXTylwBEiTVx8pcAgz0u85cAAHUNiQUm85cARIk1I/OX
				AA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - i386_init - remove rdmsr</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				uZkBAAAPMkjB4iCJxkgJ1rmYAQAADzJIweIgicBICcK/
				WAIxBTHJRTHA
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				Zg8fhAAAAAAAZg8fhAAAAAAAZg8fhAAAAAAAZg8fhAAA
				AAAAZg8fRAAA
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - replace skylake with zen</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				RIug0AEAAIuY1AEAAEiNPeuNXgDo2gMAAEiFwLkANm4B
				SA9FyEiJyEkPr8RFMf8x0kj380iJBQCrhQBIiQUhq4UA
				SLrbNLbXgt4bQ0iJyEj34kjB6hJpwkBCDwApwUiNPaeN
				XgAxwInWicpMieFJidjobTNXAEiLHeaqhQA=
				</data>
				<key>MatchBuild</key>
				<string>17G65,17G66</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				uWQAAcAPMg+2yInGwe4Ig+Y/RTH/MdJIichI9/ZIicZI
				acYAwusLSAH2SIkFCquFADHSSPf2SInDSIkdI6uFAEiJ
				NQyrhQBmDx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAABm
				Dx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - replace skylake with zen</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				RIug0AEAAIuY1AEAAEiNPceBXgDo2gMAAEiFwLkANm4B
				SA9FyEiJyEkPr8RFMf8x0kj380iJBQCThQBIiQUhk4UA
				SLrbNLbXgt4bQ0iJyEj34kjB6hJpwkBCDwApwUiNPYOB
				XgAxwInWicpMieFJidjoXSRXAEiLHeaShQA=
				</data>
				<key>MatchBuild</key>
				<string>17G5019</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				uWQAAcAPMg+2yInGwe4Ig+Y/RTH/MdJIichI9/ZIicZI
				acYAwusLSAH2SIkFCpOFADHSSPf2SInDSIkdI5OFAEiJ
				NQyThQBmDx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAABm
				Dx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - replace skylake with zen</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				RIug0AEAAIuY1AEAAEiNPWqsZgDo8AMAAEiFwLkANm4B
				SA9FyEiJyEkPr8Qx0kj380iJBenFkABIiQUKxpAASLrb
				NLbXgt4bQ0iJyEj34kUx/0jB6hJpwkBCDwApwUiNPSas
				ZgAxwInWicpMieFJidjoQ6teAEiLHczFkAA=
				</data>
				<key>MatchOS</key>
				<string>10.14.1</string>
				<key>Replace</key>
				<data>
				uWQAAcAPMg+2yInGwe4Ig+Y/RTH/MdJIichI9/ZIicZI
				acYAwusLSAH2SIkF8MWQADHSSPf2SInDSIkdCcaQAEiJ
				NfLFkABmDx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAABm
				Dx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - replace skylake with zen</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				RIug0AEAAIuY1AEAAEiNPTqZZgDo8AMAAEiFwLkANm4B
				SA9FyEiJyEkPr8Qx0kj380iJBSmokABIiQVKqJAASLrb
				NLbXgt4bQ0iJyEj34kUx/0jB6hJpwkBCDwApwUiNPfaY
				ZgAxwInWicpMieFJidjos5heAEiLHQyokAA=
				</data>
				<key>MatchOS</key>
				<string>10.14.3</string>
				<key>Replace</key>
				<data>
				uWQAAcAPMg+2yInGwe4Ig+Y/RTH/MdJIichI9/ZIicZI
				acYAwusLSAH2SIkFMKiQADHSSPf2SInDSIkdSaiQAEiJ
				NTKokABmDx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAABm
				Dx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - replace skylake with zen</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				SInISQ+vx0Ux7THSSff0SInGSIkFA2eQAEi62zS214Le
				G0NIichI9+JIiTUUZ5AASMHqEmnCQEIPACnBSI09QWpm
				ADHAidaJykyJ+U2J4OjgcF4ASIsd6WaQAA==
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				uWQAAcAPMg+2yInGwe4Ig+Y/MdJIichI9/ZIicZIaf4A
				wusLSAH2SIk97maQADHSSIn4SPf2SInDSIkdBGeQAEiJ
				Ne1mkABmDx+EAAAAAABmDx+EAAAAAABmkA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - replace skylake with zen part 2</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				RIu70AEAAESLo9QBAAA=
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				SInY6UACAABmDx9EAAA=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - tsc_init - hardset tsc </string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				SIkFlGWQAA==
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				TIkllGWQAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_init - remove version check and panic</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				JfwAAACD+BM=
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.x</string>
				<key>Replace</key>
				<data>
				JfAAAADrI5A=
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_interrupt - skip checks and prevent panic</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				gz2UlnAAAHQK
				</data>
				<key>MatchBuild</key>
				<string>17G65,17G66</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				60gPH4AAAAAA
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_interrupt - skip checks and prevent panic</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				gz2UfnAAAHQK
				</data>
				<key>MatchBuild</key>
				<string>17G5019</string>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				60gPH4AAAAAA
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_interrupt - skip checks and prevent panic</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				gz2UmHsAAHQK
				</data>
				<key>MatchOS</key>
				<string>10.14.1</string>
				<key>Replace</key>
				<data>
				60gPH4AAAAAA
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_interrupt - skip checks and prevent panic</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				gz3UensAAHQK
				</data>
				<key>MatchOS</key>
				<string>10.14.3</string>
				<key>Replace</key>
				<data>
				60gPH4AAAAAA
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_interrupt - skip checks and prevent panic</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				gz3VWHsAAHQK
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				60gPH4AAAAAA
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - mtrr_update_action - fix PAT</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				icCB4v//8P+BygAAAQC5dwIAAA==
				</data>
				<key>MatchOS</key>
				<string>10.13.6,10.14.1,10.14.3</string>
				<key>Replace</key>
				<data>
				uXcCAAC4BgEHALoGAQcADx9AAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - mtrr_update_action - fix PAT</string>
				<key>Disabled</key>
				<false/>
				<key>Find</key>
				<data>
				icCB4v//AP+BygAAAQC5dwIAAA==
				</data>
				<key>MatchOS</key>
				<string>10.14.4</string>
				<key>Replace</key>
				<data>
				uXcCAAC4BgEHALoGAQcADx9AAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - lapic_configure - remove config_mca and add extra lapic_write</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				dSlIiwXyZoUAvzUAAAD/UAgl//j+/42wAAcAAEiLBdhm
				hQC/NQAAAP9QEEiLBclmhQCLNRs2bACDxg2/MgAAAP9Q
				EEiLBbFmhQCLNQM2bACDxg+/NAAAAP9QEEiLBZlmhQCL
				Nes1bACDxgy/MwAAAP9QEIoFMmaLAITAdQXoqTL//4M9
				OmaLAAB0GEiLBWlmhQCLNbs1bACDxgm/LwAAAP9QEA==
				</data>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				SIsF9GaFAL81AAAAdRz/UAgl//j+/42wAAcAAEiLBdhm
				hQC/NQAAAOsFvgAHAQD/UBBIiwXCZoUAizUUNmwAg8YN
				vzIAAAD/UBBIiwWqZoUAizX8NWwAg8YPvzQAAAD/UBBI
				iwWSZoUAizXkNWwAg8YMvzMAAAD/UBBmDx+EAAAAAABm
				Dx+EAAAAAABmDx+EAAAAAABmDx+EAAAAAAAPH0QAAA==
				</data>
			</dict>
			<dict>
				<key>Comment</key>
				<string>algrey - cpu_topology_sort -disable cpshadows</string>
				<key>Disabled</key>
				<true/>
				<key>Find</key>
				<data>
				SIsF34BtAEiNDYgI2f9IiYhYAQAAQbcBg33IAQ+EhQAA
				AEyLbdBB9sUBdSk=
				</data>
				<key>MatchOS</key>
				<string>10.13.6</string>
				<key>Replace</key>
				<data>
				QbcBTIttyEyJbdDpAAAAAGYPH4QAAAAAAGYPH4QAAAAA
				AEyLbdAPH0AA63s=
				</data>
			</dict>
		</array>