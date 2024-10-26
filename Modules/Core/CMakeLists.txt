project(Cango.ByteCommunication.Core)

AddCXXModule(
	NAME "Core"
	NAMESPACE "Cango::ByteCommunication"
	CXX_STANDARD 26
	HEADER_DIR Headers
	SOURCE_DIR Sources
	TESTER_DIR Testers
	LINKS
		"Cango::TaskDesign"
		"Cango::CommonUtils"
)
