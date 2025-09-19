.PHONY: all debug release clean

# Объявление переменных
CXX = g++                          # Компилятор C++
RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS = -g -O0 -Wall
RELEASE_EXEC = Kazino-Royal        # Имя релизного исполняемого файла (можно без пробелов)
DEBUG_EXEC = Kazino-Royal-dbg      # Имя отладочного исполняемого файла
SOURCE = Kazino-Royal.cpp          # Имя исходного файла

# Цели
all: debug release

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): $(SOURCE)
	$(CXX) $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC)

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): $(SOURCE)
	$(CXX) $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC) *.o
