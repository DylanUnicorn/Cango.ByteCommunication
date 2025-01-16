project(Cango.ByteCommunication.BoostImplementations)

AddCXXModule(
	NAME "BoostImplementations"
	NAMESPACE "Cango::ByteCommunication"
	CXX_STANDARD 20
	HEADER_DIR Headers
	SOURCE_DIR Sources
	TESTER_DIR Testers
	LINKS
		"fmt::fmt"
		"spdlog::spdlog"
		"Boost::system"
		"Cango::ByteCommunication::Core"
)
