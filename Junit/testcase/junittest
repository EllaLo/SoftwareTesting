import java.util.*;

import org.junit.Test;
import static org.junit.Assert.assertEquals;
import org.junit.runner.RunWith;
import org.junit.runners.Parameterized;
import org.junit.runners.Parameterized.Parameters;

@RunWith(value = Parameterized.class)
public class junittest<T extends Comparable<? super T>> {
    List<T> list;
    T expected;

    public junittest(List<T> list, T expected) {
        this.list = list;
        this.expected = expected;
    }

    @Parameters(name = "{index}: Distant.distant({0})={1}")
    public static Iterable<Object[]> data1() {
        return Arrays.asList(new Object[][] { { Arrays.asList(4,5,6,7,8,9),4 }, { Arrays.asList("x", "y", "z"), "x" },
          { Arrays.asList("cat", "dog", "ant"), "ant" }});
    }

    @Test
    public void testDistant() {
        T result = Min.min(list);
        assertEquals(expected, result);
    }
}
